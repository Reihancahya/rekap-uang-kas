<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-lg-12">
                <h2 class="text-center my_4">RIWAYAT PEMASUKAN KAS</h2>
                <div class="my-3">
                    <input type="search" class="form-control-lg rounded-5">
                </div>
                <div class="my-3 text-muted">menampilkan 1 dari 36</div>
                <table class="table">
                    <thead>
                        <tr>
                           
                            <td>NO</td>
                            <td>NAMA</td>
                            <td>WAKTU</td>
                            <td>TANGGAL</td>
                            <td>NOMINAL</td>
                            <td>TOTAL</td>
                        </tr>
                    </thead>
                    <tbody>
                        <tr v-for="(visitor, i) in visitors" :key="i">
                            <td>{{ i + 1 }}</td>
                            <td>{{ visitor.nama }}</td>
                            <td>{{ visitor.keanggotaan.nama }}</td>
                            <td>{{ visitor.tanggal }},{{ visitor.waktu }}</td>
                            <td>{{ visitor.keperluan.nama }}</td>
                        </tr>
                    </tbody>
                </table>
                </div>
            </div>
        </div>
</template>
<script setup>
const supabase = useSupabaseClient()

const visitors = ref([])
const getPembayaran = async () => {
    const { data, error } = await supabase.from('Pembayaran').select('*,keanggotaan(*), keperluan(*)')
    if (data) visitors.value = data
}
const totalPembayaran = async () => {
    const { data, count } = await supabase.from('Pembayaran')
    .select("*", {count: 'exact'})
    if (data) jumlah.value = count
}
onMounted(() => {
    getPengunjung()
    totalPengunjung()
})</script>
