<template>
	<md-card id="signin-card">
	<form id="signin-form" novalidate @submit.stop.prevent="">
		<span id="headline" class="md-headline">登陆</span>
		<md-input-container>
			<label>用户名</label>
			<md-input required></md-input>
		</md-input-container>
		<md-input-container>
			<label>密码</label>
			<md-input required></md-input>
		</md-input-container>
		<router-link to="/SignUp">
			<md-button id="signup-button" class="md-raised md-primary">注册</md-button>
		</router-link>
		<md-button id="signin-button" class="md-raised md-primary">登陆</md-button>
	</form>
</md-card>
</template>

<script>
	export default {
	}
</script>

<style scoped>
	#signin-card {
		width: 320px;
		margin: 32px auto;
		padding: 24px 48px;
	}
	#signin-button, #signup-button {
		margin: 16px 8px;
	}
	#headline {
		margin-bottom: 16px;
	}
</style>
