<template>
  <div>
      <CRow><CCol></CCol><CCol sm="6">
      <CCard>
          <CForm>
          <CCardHeader>
              <strong>ຟອມລົງທະບຽນນັກກິລາ</strong>
          </CCardHeader>
          <CCardBody>
              <CRow>
                  <CCol sm="3">
                      <CSelect label = "ຄຳນຳໜ້າ" 
                        :options="options"
                        placeholder="ທ້າວ/ນາງ"
                        required/>
                  </CCol>
              </CRow>
              <CRow>
                  <CCol sm="6">
                      <CInput label="ຊື່ແທ້"
                  description="ໃສ່ເປັນພາສາລາວ"
                  placeholder="ຈອນ"
                  required/>
                  </CCol>
                  <CCol sm="6">
                      <CInput label="ນາມສະກຸນ"
                  description="ໃສ່ເປັນພາສາລາວ"
                  placeholder="ວິກ"
                  required/>
                  </CCol>
              </CRow>
              <CRow>
                  <CCol sm="6">
                      <CInput label="ຊື່ຫຼິ້ນ"
                  description="ໃສ່ເປັນພາສາລາວ"
                  placeholder="ປ໊ອກກີ້"/>
                  </CCol>
              </CRow>
              <CRow>
                  <CCol sm="6">
                      <CInput label="ເບີໂທລະສັບ"
                  placeholder="020xxxxxxxx"
                  required/>
                  </CCol>
              </CRow>
              <CRow>
                  <CCol sm="6">
                      <CInput label="Facebook"
                  placeholder="Lunk Soutthichak"/>
                  </CCol>
              </CRow>
              <CRow>
                  <CCol sm="6">
                      <CInputCheckbox
                      v-for="(option, optionIndex) in sports"
                      :key="key + option"
                      :label="option"
                      :value="option"
                      :custom="key > 1"
                      :name="`Option 1${key}`"
                      :checked="optionIndex === key"
                      :inline="key % 2 === 1"
                      />
                  </CCol>
              </CRow>
              
          </CCardBody>
          <CCardFooter>
              <center>
                  <CButton type="submit" size="sm" color="primary"><CIcon name="cil-check-circle"/> Submit</CButton>
                  <CButton type="reset" size="sm" color="danger"><CIcon name="cil-ban"/> Reset</CButton>
              </center>
          </CCardFooter>
          </CForm>
      </CCard>
      </CCol>
      <CCol></CCol>
      </CRow>
  </div>
</template>

<script>
export default {
    name: 'Forms',
    data () {
        return {
            options: ['ທ້າວ', 'ນາງ'],
            sports: ['ຕີບານ', 'ເຕະບານ', 'ເຕະກະຕໍ້']
        }
    }
}
</script>

<style>

</style>