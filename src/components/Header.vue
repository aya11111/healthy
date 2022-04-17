<template>
    <div>
        <div class="container">
            <header>
                <div class="brand">
                    <router-link to="/"><fontAwesome icon="leaf"/>healthy</router-link>
                </div>
                <nav class="navbar">
                    <router-link to="/">home</router-link>
                    <router-link to="/shop">shop</router-link>
                    <router-link to="/about">about</router-link>
                    <router-link to="/review">review</router-link>
                    <router-link to="/blog">blog</router-link>
                    <router-link to="/contact">contact</router-link>
                </nav>
                <div class="icons">
                    <div @click="mobilemenu()" id="menu-btn"><fontAwesome icon="bars"/></div>
                    <div @click="search()" id="search"><fontAwesome icon="magnifying-glass" /></div>
                    <div @click="login()" id="user-btn"><fontAwesome icon="user"/></div>
                </div>

                <form action="" class="search-form">
                    <input type="search" placeholder="search here" id="search-box" ref="input" class="lol">
                    <label for="search-box"><fontAwesome icon="magnifying-glass"/></label>
                </form>

                <form action="" class="login-form">
                    <h2>login form</h2>
                    <input type="email" placeholder="your email" name="email">
                    <input type="password" placeholder="your password" name="password">
                    <div>
                        <input type="checkbox" id="log-remember">
                        <label for="log-remember">remember me</label>
                    </div>
                    <input type="submit" value="login now">
                    <p>forget password? <a href="#">click here</a></p>
                    <p>don't have an account? <a href="#">create one</a></p>
                </form>
            </header>
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        search() {
            this.$el.querySelector(".search-form").classList.toggle("active");
            this.$el.querySelector(".login-form").classList.remove("active");
            this.$el.querySelector(".navbar").classList.remove("active");
            
        },

        login() {
            this.$el.querySelector(".login-form").classList.toggle("active");
            this.$el.querySelector(".search-form").classList.remove("active");
            this.$el.querySelector(".navbar").classList.remove("active");
        },

        mobilemenu() {
            this.$el.querySelector(".navbar").classList.toggle("active");
            this.$el.querySelector(".login-form").classList.remove("active");
            this.$el.querySelector(".search-form").classList.remove("active");
        }
    }
}
</script>