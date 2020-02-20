<template>
  <CContainer class="d-flex align-items-center min-vh-100">
    <CRow>
      <CCol md="12">
          <CCard class="p-4">
            <CCardBody>
              <CForm>
                <center><img src="../../../public/img/brand/sw-logo-229x109.png"></center>
                <h3>ລະບົບສະໝັກນັກກິລາພາກວິຊາ CEIT</h3>
                <p class="text-muted">Sign In to your account</p>
                <CInput
                  placeholder="Username"
                  autocomplete="username email"
                >
                  <template #prepend-content><CIcon name="cil-user"/></template>
                </CInput>
                <CInput
                  placeholder="Password"
                  type="password"
                  autocomplete="curent-password"
                >
                  <template #prepend-content><CIcon name="cil-lock-locked"/></template>
                </CInput>
                <CRow>
                  <CCol col="6">
                    <a href="#/dashboard"><CButton color="primary" class="px-4">Login</CButton></a>
                  </CCol>
                  <CCol col="6" class="text-right">
                    <CButton color="link" class="px-0">Forgot password?</CButton>
                  </CCol>
                </CRow>
              </CForm>
            </CCardBody>
          </CCard>
      </CCol>
    </CRow>
  </CContainer>
</template>

<script>
export default {
  name: 'Login',
  data() {

  }
}
</script>
