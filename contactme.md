---
layout: page
title: Contact form
permalink: /contactme/
---

I would love to hear from you. Any query, any suggestion or feedback would be great!


<form id="contact-form" class="form-horizontal" action="https://getsimpleform.com/messages?form_api_token=b6d4be9b039b666b3311e1ddcbfb577c" method="POST" enctype="multipart/form-data">
       <fieldset>

            <div class="form-group">
                <label class="col-lg-2 control-label" for="name">Name:</label>
                <div class="col-lg-10">
                <input type="text" placeholder="Your name" id="name" class="form-control" name="name" tabindex="1"/>
                </div>
            </div>
            <div class="form-group">
                <label class="col-lg-2 control-label" for="email">Email:</label>
                <div class="col-lg-10">
                <input type="email" placeholder="Your email" id="email" class="form-control" name="email" tabindex="2"/>
                </div>
            </div>
            <div class="form-group">
                <label class="col-lg-2 control-label" for="message">Message:</label>
                <div class="col-lg-10">
                <textarea class="contact-textarea" placeholder="Your message" class="form-control" rows="8" id="message" name="message" tabindex="3"></textarea>
                </div>
            </div>

           <div class="form-group">
           <div class="col-lg-10 col-lg-offset-2">  
         <input type="submit" class="btn btn-primary" value="Send" id="submit"/>
         </div>
         </div>
        <input type="hidden" name='redirect_to' value="//petkovicm.github.io/" />
    </fieldset>  
</form>
