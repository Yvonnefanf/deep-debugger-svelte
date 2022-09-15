<style>
  #loginContainer {
    display: none;
    position: absolute;
    width: 100%;
    height: 100vh;
    background: linear-gradient(35deg, #bb313e25, #bb313e25, #d7222925, #dd4a1625, #e4761525, #f5c50025, #f0e92725, #b1ce2425, #48a93525, #03944525, #157c4f25, #176a5825, #1b556325, #1d386f25, #1d386f25, #20277825, #52266325, #8a244b25);
    text-align: center;

  }

  .login-page-title {
    position: absolute;
    text-align: center;
    top: 20%;
    left: 50%;
    width: 350px;
    margin-left: -90px;
  }

  .login-card {
    width: 300px;
    height: 250px;
    position: fixed;
    top: 30%;
    left: 50%;
    margin-left: -150px;
    text-align: center;
    padding: 20px 80px 50px 80px;
    box-shadow: 0 3px 15px rgb(0 0 0 / 20%);
    background: rgba(255, 255, 255, 0.3);
  }

  .login-input {
    height: 30px;
    width: 200px;
  }

  .login-item {
    margin: 10px 0;
    display: flex;
    justify-content: space-between;
    width: 100%;
    line-height: 36px;
  }

  #loginBtn,
  #registerBtn,
  button {
    width: 40%;
    height: 32px;
    line-height: 32px;
    margin: 10px 0;
    background: #560731;
    border: none;
    color: #fff;
  }

  .footer {
    display: flex;
    justify-content: space-between;
  }

  .choose-task {
    white-space: nowrap;
  }
</style>


<div id="loginContainer">
	<h1 class="login-page-title">Embedding Projector</h1>
	<div class="login-card">
		<h2>User Login</h2>
		<div class="login-item">
			<span>username:</span><input class="login-input" id="loginInput" />
		</div>
		<div class="login-item">
			<span>password:</span><input type="password" class="login-input" id="passwordInput" />
		</div>
		<div class="login-item">
			<span>ip:host</span><input
				type="input"
				class="login-input"
				id="ipAddressInput"
				value="localhost:5001"
			/>
		</div>
		<div class="footer">
			<button id="loginBtn" style="width: 100%;" class="ink-button">Login</button>
			<button id="registerBtn" style="visibility: hidden;width: 0;" class="ink-button"
				>Register</button
			>
		</div>
		<div class="choose-task">
			task:
			<input type="radio" name="task" value="anormaly detection" checked="checked" /> Fault
			Localization
			<input type="radio" name="task" value="active learning" />Sample Selection
		</div>
	</div>
</div>

