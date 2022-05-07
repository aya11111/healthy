<template>
<div>
    <section class="contact" data-aos="fade-up">
        <div class="sub-background">
            <div class="page-details">
                <h2>contact us</h2>
                <p><router-link to="/">home</router-link> >> contact</p>
            </div>
        </div>
        <div class="container">
            <div class="contact-details">
                <div class="item" data-aos="fade-left">
                    <div class="icon"><fontAwesome icon="phone"/></div>
                    <h3>our number</h3>
                    <p>+111 111 222</p>
                    <p>+333 777 555</p>
                </div>
                <div class="item" data-aos="fade-up">
                    <div class="icon"><fontAwesome icon="message"/></div>
                    <h3>our email</h3>
                    <p>aaaaa@gmail.com</p>
                    <p>bbbbb@gmail.com</p>
                </div>
                <div class="item" data-aos="fade-right">
                    <div class="icon"><fontAwesome icon="location-dot"/></div>
                    <h3>our address</h3>
                    <p>egypt cairo</p>
                </div>
            </div>
            <div class="contact-body">
                <form action="" data-aos="fade-right">
                    <h3>get in touch</h3>
                    <input type="text" name="name" placeholder="your name">
                    <input type="email" name="email" placeholder="your email">
                    <input type="number" name="number" placeholder="your number">
                    <input type="text" name="subject" placeholder="your subject">
                    <textarea placeholder="your message" name="message"></textarea>
                    <input type="submit" value="send message">
                </form>
                <div class="map" data-aos="fade-left">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d110502.76973643026!2d31.18842340425844!3d30.05946989027819!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x14583fa60b21beeb%3A0x79dfb296e8423bba!2sCairo%2C%20Cairo%20Governorate!5e0!3m2!1sen!2seg!4v1649549714459!5m2!1sen!2seg" width="600" height="450" style="border:0;"  loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                </div>
            </div>
        </div>
    </section>
</div>
</template>
