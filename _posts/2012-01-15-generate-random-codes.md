---
layout: post
title:  Generate random codes and write to CSV file
categories: [snippet]
tags: [ruby]
---

    require 'csv'
    charset = %w{0 1 2 3 4 5 6 7 8 9 a b c d e f g h i j k l m n o p q r s t u v w x y z}

    CSV.open("codes-single.csv", "w") do |csv|
      100.times.map do
        csv << [(0...8).map{ charset.to_a[rand(charset.size)] }.join]
      end
    end
