<template>
  <!-- Section -->
  <div class="section section-pad">
    <div class="container">
      <div class="tab-custom">
        <div class="row">
          <div class="col-md-4 col-md-offset-4  col-sm-6 col-sm-offset-3">
            <ul class="nav nav-tabs ucap" id="loginreg-form">
              <li class="active"><a href="#tab1" data-toggle="tab">Log In</a></li>
              <li><a href="#tab2" data-toggle="tab">Register</a></li>
            </ul>
          </div>
        </div>
        <div class="gaps size-2x"></div>
        <!-- Tab panes -->
        <div class="tab-content no-pd">
          <div class="tab-pane fade in active" id="tab1">
            <div class="row">
              <div class="col-md-6 col-md-offset-3 col-sm-8 col-sm-offset-2">
                <h3 class="heading-lead center">Login Your Account</h3>
                <form class="form-signup" action="action.php" method="post">
                  <div class="form-results"></div>
                  <div class="form-group">
                    <div class="form-field form-m-bttm">
                      <input name="signup-email" type="email" placeholder="Email *" class="form-control required email" aria-required="true">
                    </div>
                  </div>
                  <div class="form-group">
                    <div class="form-field">
                      <input name="signup-passkey" type="password" placeholder="Password *" class="form-control required" aria-required="true">
                    </div>
                  </div>
                  <button type="submit" class="btn btn-alt">Log In</button>
                  <span class="gaps"></span>
                  <p class="small">Not registered? <a class="switch-tab" data-tabnav="loginreg-form" href="#tab2" data-toggle="tab">Register here</a></p>
                </form>
              </div>
            </div>
          </div>
          <div class="tab-pane fade" id="tab2">
            <div class="row">
              <div class="col-md-6 col-md-offset-3 col-sm-8 col-sm-offset-2">
                <h3 class="heading-lead center">Register An Account</h3>
                <form class="form-signup" action="action.php" method="post">
                  <div class="form-results"></div>
                  <div class="form-group">
                    <div class="form-field form-m-bttm">
                      <input name="signup-name" type="text" placeholder="Name *" class="form-control required" aria-required="true">
                    </div>
                  </div>
                  <div class="form-group">
                    <div class="form-field form-m-bttm">
                      <input name="signup-email" type="email" placeholder="Email *" class="form-control required email" aria-required="true">
                    </div>
                  </div>
                  <div class="form-group">
                    <div class="form-field">
                      <input name="signup-passkey" type="password" placeholder="Password *" class="form-control required" aria-required="true">
                    </div>
                  </div>
                  <div class="form-group">
                    <div class="form-field">
                      <input name="signup-passkey-confirm" type="password" placeholder="Confirm Password *" class="form-control required" aria-required="true">
                    </div>
                  </div>
                  <div class="form-group">
                    <div class="form-field">
                      <input type="checkbox" name="signup-term"> <span> I accept and agree with the terms of the <a href="#">User Agreement</a>.</span>
                    </div>
                  </div>

                  <button type="submit" class="btn btn-alt">Signup</button>
                  <span class="gaps"></span>
                  <p class="small">Already registered? <a class="switch-tab" data-tabnav="loginreg-form" href="#tab1" data-toggle="tab">Login here</a></p>
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>	
  </div>
  <!-- End Section -->
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
