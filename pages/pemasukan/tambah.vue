<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-lg-12">
                <h2 class="text-center my-4">FORM PEMBAYARAN KAS</h2>
                    <div class="mb-3">
                    </div>
                    <div class="mb-3">
                        <select class="form-control form-control-lg form-select rounded-5">
                            <option value="">NAMA</option>
                            <option value="">Ahmad Rama</option>
                            <option value="">Ainy</option>
                            <option value="">Alfi</option>
                            <option value="">Alsya </option>
                            <option value="">Aura </option>
                            <option value="">Dita </option>
                            <option value="">Elisa </option>
                            <option value="">Fadlan </option>
                            <option value="">Fajar </option>
                            <option value="">Fauzan </option>
                            <option value="">Guntur </option>
                            <option value="">Herpa </option>
                            <option value="">Hilal</option>
                            <option value="">Melva</option>
                            <option value="">Miftah</option>
                            <option value="">mirna</option>
                            <option value="">Nouvel </option>
                            <option value="">Randid </option>
                            <option value="">Reihan</option>
                            <option value="">Ridho</option>
                            <option value="">Rifat</option>
                            <option value="">Rike</option>
                            <option value="">Rivald </option>
                            <option value="">Ronald</option>
                            <option value="">Salma</option>
                            <option value="">Sasta</option>
                            <option value="">Seli</option>
                            <option value="">Siti </option>
                            <option value="">Sofwa </option>
                            <option value="">Tejar</option>
                            <option value="">Tiara</option>
                            <option value="">Wildan</option>
                            <option value="">Yogi</option>
                            <option value="">Yuliana </option>
                        </select>
                    </div>
                    <div class="mb-3">
                        <div class="row">
                            <div class="col-mb-3">
                                <input type="text" class="form-control form-control-lg  rounded-5" placeholder="MASUKKAN NOMINAL">
                            </div> 
                        </div>
                    </div>
                    <Nuxt-Link to="/">
                        <button type="submit" class="btn btn-outline-danger rounded-6" style="color: black; font-family: lnria-serif">BATAL</button>
                    </Nuxt-Link>
                    <Nuxt-Link to="/laporan">
                        <button type="submit" class="btn btn-outline-primary rounded-6" style="color: black; font-family: lnria-serif">KIRIM</button>
                    </Nuxt-Link>
            </div>
        </div>
    </div>
</template>