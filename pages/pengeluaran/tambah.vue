<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-lg-12">
                <h2 class="text-center my-4">FORM REKAP PENGELUARAN KAS</h2>
                    <div class="mb-3">
                    </div>
                    <div class="mb-3">
                        <input type="text" class="form-control form-control-lg rounded-5" placeholder="KETERANGAN">
                    </div>
                    <div class="mb-3">
                        <div class="row">
                            <div class="col-mb-3">
                                <input type="text" class="form-control form-control-lg  rounded-5" placeholder="MASUKKAN NOMINAL">
                            </div> 
                        </div>
                    </div>
                    <input type="text" class="form-control form-control-lg  rounded-5" placeholder="TAMBAHAN">
            </div>
        </div>
    </div>
    <Nuxt-Link to="/laporan">
    <button type="submit" class="btn btn-outline-primary rounded-6" style="color: black; font-family: lnria-serif">BATAL</button>
    </Nuxt-Link>
</template>
  