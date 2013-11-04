---
layout: default
title:  Render Transactional Email in Browser
categories: [tips]
tags: [rails]
---

If you have something like this in `routes.rb`

    match "emails/:email_file" => "emails#show"

Then in the emails controller, you can do like so:

    def show
      render params[:email_file], layout: "mailer"
    end

This way, you can view how any transactional email look in the browser. Of course, to really test any HTML email, you need to do the inbox test.
