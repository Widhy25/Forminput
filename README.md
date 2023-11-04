
        <?php } else {         
          if ($formulir->foto=='Ya' || $formulir->foto_full=='Ya' || $formulir->rapor=='Ya' || $formulir->akte_kelahiran=='Ya' || $formulir->kartu_keluarga=='Ya' || $formulir->skl_skhu=='Ya' || $formulir->skd=='Ya' || $formulir->sktm=='Ya' || $formulir->ktp_ortu=='Ya' || $formulir->sptjm=='Ya' || $formulir->sp=='Ya' || $formulir->kartu_bantuan=='Ya' || $formulir->berkaslain=='Ya') { ?>            
            <form action="uploadberkas" method="post" enctype="multipart/form-data">
                <div class="col-xs-12 col-md-12">
                  <?php if ($formulir->foto=='Ya'){ ?>
                      <div class="form-group">
                        <label for="varchar">Foto Berwarna 3x4</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="Foto 3x4"/>
                      </div>             
                  <?php } ?>
                  <?php if ($formulir->foto_full=='Ya'){ ?>
                      <div class="form-group">
                        <label for="varchar">Foto Seluruh Badan</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="Foto Seluruh Badan"/>
                      </div>             
                  <?php } ?>
                  <?php if ($formulir->skl_skhu=='Ya'){ ?>  
                      <div class="form-group">
                        <label for="varchar">SKL/SKHU/Ijazah</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="SKL/SKHU/Ijazah" />
                      </div>      
                  <?php } ?>
                  <?php if ($formulir->rapor=='Ya'){ ?>
                      <div class="form-group">
                        <label for="varchar">Nilai Rapor Semester 1-5</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="Nilai Rapor/Semester"/>
                      </div>             
                  <?php } ?>
                  <?php if ($formulir->akte_kelahiran=='Ya'){ ?>
                      <div class="form-group">                      
                        <label for="varchar">Akta Kelahiran</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="Akta Kelahiran" />  
                      </div>
                  <?php } ?>
                  <?php if ($formulir->kartu_keluarga=='Ya'){ ?>
                      <div class="form-group">
                        <label for="varchar">Kartu Keluarga</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />  
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="Kartu Keluarga" /> 
                      </div>
                  <?php } ?>  
                  <?php if ($formulir->ktp_ortu=='Ya'){ ?>
                      <div class="form-group">
                        <label for="varchar">KTP Orangtua</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />  
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="KTP Orangtua" /> 
                      </div>
                  <?php } ?>
                  <?php if ($formulir->sptjm=='Ya'){ ?>
                      <div class="form-group">
                        <label for="varchar">Surat Pertanggungjawaban Mutlak Orangtua</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />  
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="Surat Pertanggungjawaban Mutlak Orangtua" /> 
                      </div>
                  <?php } ?> 
                  <?php if ($formulir->sp=='Ya'){ ?>
                      <div class="form-group">
                        <label for="varchar">Surat Penugasan dari Instansi</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />  
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="Surat Penugasan dari Instansi" /> 
                      </div>
                  <?php } ?>                                       
                  <?php if ($formulir->skd=='Ya'){ ?>
                      <div class="form-group">
                        <label for="varchar">Surat Keterangan Domisili</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />  
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="Surat Keterangan Domisili" />                          
                      </div>                   
                  <?php } ?> 
                  <?php if ($formulir->sktm=='Ya'){ ?>
                      <div class="form-group">
                        <label for="varchar">Surat Keterangan Tidak Mampu</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />  
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="Surat Keterangan Tidak Mampu" />                          
                      </div>                   
                  <?php } ?>    
                  <?php if ($formulir->kartu_bantuan=='Ya'){ ?>
                      <div class="form-group">
                        <label for="varchar">Kartu PKH/KPS/KIP</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />  
                        <input type="hidden" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" value="Kartu PKH/KPS/KIP" />                          
                      </div>                   
                  <?php } ?>                                  
                </div>                    
                  <?php if ($formulir->berkaslain=='Ya'){ ?>
                    <div class="col-xs-12 col-md-6"> 
                      <div class="form-group">
                        <label for="varchar">Berkas lainnya</label>
                        <input type="hidden" class="form-control" name="id_peserta[]" value="<?php echo $nomer->id_peserta; ?>"/>
                        <input type="file" class="form-control" name="berkas[]" />
                      </div>
                    </div>                       
                    <div class="col-xs-12 col-md-6"> 
                      <div class="form-group">
                        <label for="varchar">Keterangan Berkas</label>                                            
                        <input type="text" class="form-control" name="keterangan_berkas[]" placeholder="Keterangan Berkas" />
                      </div> 
                    </div>   
                  <?php } ?> 
                  <div class="col-xs-12 col-md-6"> 
                    <div class="form-group">    
                        <button type="submit" class="<?= $this->config->item('botton')?>">Upload Berkas</button>
                    </div>
                  </div>              
            </form> 
            
        </div> 
              <div class="callout callout-info">
                Berkas yang akan diupload harus sesuai ketentuan
                <li>format berkas : gif/jpg/png/pdf</li>
                <li>ukuran max : 500 kb</li>
                <?php if ($formulir->berkaslain=='Ya'){ ?>
                  <li>ulangi proses upload berkas lainnya jika masih ada berkas yang perlu di upload</li>
                <?php } ?>                 
              </div>  
          <?php } else { ?>
          <div class="col-xs-12 col-md-12">  
            <div class="callout callout-info">
              Berkas pendukung di serahkan langsung ke Panitia PPDB disertai bukti pendaftaran
            </div> 
          </div>             
          <?php } ?>
        <?php } ?>   
      <?php } else { ?>
        <div class="col-xs-12 col-md-12">  
          <div class="callout callout-info">
            Silahkan melakukan pengisian formulir pendaftaran terlebih dahulu
          </div> 
        </div> 
      <?php } ?>                                        
      </div>
    </div>
  </div>
</div>
<!-- end Modal Berkas -->

<!-- DataTables -->
<script src="<?= base_url('assets/bower_components/jquery/dist/jquery.min.js');?>"></script>  
<script src="<?= base_url('assets/bower_components/datatables.net/js/jquery.dataTables.min.js');?>"></script>
<script src="<?= base_url('assets/bower_components/datatables.net-bs/js/dataTables.bootstrap.min.js');?>"></script>  

<script type="text/javascript">
  $(document).ready(function() {
    $('#mytable').DataTable();
  });
</script>
