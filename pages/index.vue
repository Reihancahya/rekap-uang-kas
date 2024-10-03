<template>
    <div class="container-fluid">
        <div class="row my-5">
            <div class="col-lg-6">
                <nuxt-link to="/siswa">
                    <div class="card bg data pemasukan rounded-5">
                        <div class="card-body">
                            <h2>SISWA PPLG2</h2>
                        </div>
                    </div>
                </nuxt-link>
            </div>
        <div class="col-lg-6">
        <nuxt-link to="pemasukan/tambah">
                <div class="card bg-pemasukan rounded-5">
                    <div class="card-body">
                        <h2>DATA PEMASUKAN</h2>
                    </div>
                </div>
        </nuxt-link>
        </div>
        <div class="col-lg-6">
        <nuxt-link to="laporan/">
                <div class="card bg-buku rounded-5">
                    <div class="card-body">
                        <h2>LAPORAN</h2>
                    </div>
                </div>
        </nuxt-link>
        </div>
        <div class="col-lg-6">
        <nuxt-link to="pengeluaran/tambah">
                <div class="card bg-buku rounded-5">
                    <div class="card-body">
                        <h2>REKAP PENGELUARAN PERMINGGU</h2>
                    </div>
                </div>
        </nuxt-link>
        </div>
    </div>
</div>
</template>
<style scoped>
.card {
    height: 250px;
    box-shadow: 1px 1px 1px #424242;
}
.card.bg-pemasukan {
    background-image: url('../assets/img/Uang-Kas-.jpg');
    background-repeat: no-repeat;
    background-position: certer center;
    background-size: cover;
}
.card.bg-laporan{
    background: url no-repeat center center;
    background-size: cover;
}
</style>