<template>
    <div>
        <footer>
            <div class="container">
                <div class="footer-item">
                    <h3>quick links</h3>
                    <ul>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/">home</router-link></li>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/shop">shop</router-link></li>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/about">about</router-link></li>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/review">review</router-link></li>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/blog">blog</router-link></li>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/contact">contact</router-link></li>
                    </ul>
                </div>
                <div class="footer-item">
                    <h3>extra links</h3>
                    <ul>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/">order</router-link></li>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/">favourite</router-link></li>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/">wishlist</router-link></li>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/">account</router-link></li>
                        <li><fontAwesome icon="arrow-right" /> <router-link to="/">terms</router-link></li>
                    </ul>
                </div>
                <div class="footer-item">
                    <h3>follow us</h3>
                    <ul>
                        <li><fontAwesome :icon="['fab', 'facebook']"/><router-link to="/">facebook</router-link></li>
                        
                        <li><fontAwesome :icon="['fab', 'twitter']" /><router-link to="/">twitter</router-link></li>
                        <li><fontAwesome :icon="['fab','instagram']" /><router-link to="/">instagram</router-link></li>
                        <li><fontAwesome :icon="['fab', 'linkedin']" /><router-link to="/">linkedin</router-link></li>
                        <li><fontAwesome :icon="['fab', 'pinterest']" /><router-link to="/">pinterest</router-link></li>
                    </ul>
                </div>
                <div class="footer-item">
                    <h3>newsletter</h3>
                    <form action="">
                        <h5>subscribe for latest updates</h5>
                        <input type="email" placeholder="type your email" name="email">
                        <input type="submit" value="subscribe">
                    </form>
                    <div class="pay">
                        <ul>
                            <li><fontAwesome :icon="['fab', 'cc-visa']" /></li>
                            <li><fontAwesome :icon="['fab', 'cc-mastercard']" /></li>
                            <li><fontAwesome :icon="['fab', 'cc-paypal']" /></li>
                            <li><fontAwesome :icon="['fab', 'cc-amazon-pay']" /></li>
                        </ul>
                    </div>
                </div>
            </div>
        </footer>
    </div>
</template>