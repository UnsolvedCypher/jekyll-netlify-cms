---
title: Contact
permalink: /contact
layout: default
heading: Contact Us
subheading: We're here to answer any questions you may have
bg-class: bg-2
---
<!-- contact form start -->
<section class="contact-form">
    <div class="container">
        <div class="row">
        <h3>If you'd like to chat with us live, use the chat  button in the bottom right during our business hours (8:30am-5:00pm EST). Or, if you prefer, drop us a message using the form below!</h3>
        </div>
        <section class="contact-form">
        <div class="row">
            <form id="contact-form" action="https://formspree.io/info@computerfulfillment.com" method="POST">
                <div class="col-md-6 col-sm-12">
                    <div class="block">

                        <div class="form-group">
                            <input name="name" type="text" class="form-control" placeholder="Your Name">
                        </div>
                        <div class="form-group">
                            <input name="email" type="text" class="form-control" placeholder="Email Address">
                        </div>
                        <!-- The below input is a spam filter- don't touch it -->
                        <input type="text" name="_gotcha" style="display:none" />
                        <!-- The below input indicates which page the form should go to after submission -->
                        <input type="hidden" name="_next" value="https://cf-site.netlify.com/thanks" />
                        <div class="form-group">
                            <input name="_subject" type="text" class="form-control" placeholder="Subject">
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-sm-12">
                    <div class="block">
                        <div class="form-group-2">
                            <textarea name="message" class="form-control" rows="3" placeholder="Your Message"></textarea>
                        </div>
                            <button class="btn btn-default" type="submit" value="Send">Send Message</button>
                    </div>
                </div>
                <div class="error" id="error">Sorry Msg dose not sent</div>
                <div class="success" id="success">Message Sent</div>
            </form>
        </div>
        <div class=" contact-box row">
            <div class="col-md-6 col-sm-12">
                <div class="block">
                    <h2>Our Headquarters</h2>

            				{% include address.html %}

                </div>
            </div>
            <div class="col-md-6 col-sm-12">
                <div class="block">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2939.8905939015526!2d-71.23131844880902!3d42.53637873183854!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89e3a0289393f48f%3A0xb92053e6094ede30!2sComputer+Fulfillment+Inc!5e0!3m2!1sen!2sus!4v1529508002946" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
                </div>
        </div>
    </div>
</section>
