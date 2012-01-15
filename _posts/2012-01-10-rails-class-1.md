---
layout: post
title :  First Ruby on Rails Class
categories : [learning]
tags : [ruby]
---

## Basic Ruby

Ruby is object-oriented language, written in C. A developer said Ruby is built as improvisation of PHP.

**Class** - A category of objects.

    class Post
      def initiate
        ...
      end
    end

**Object** - An instance of the class.

**Constructor** - A special method to create objects.

    post = Post.new("Resolution")

**Method** - Process objects. There are class methods and instance methods.

    def to_s
      puts "#{title}"
    end

## Array & Hash

**Array** - An indexed collection that store objects, accessible by keys. The key is an integer.

    a = ['queen','guns','roses','beatles']
    a[0] # => "queen"
    a[3] # => "beatles"
    
**Hash** - A collection of key-value pair. The value is accessible by the key.

    band = {
      'queen' => 'bohemian rhapsody',
      'aerosmith' => 'i don't want to miss a thing',
      'chicago' => 'if you leave me now'
    }
    
    puts band['queen'] # => "bohemian rhapsody"

## Symbols

A symbol is a constant name that is unique throughout the system. Can be used as hashes key.

    config = {
      :start => true,
      :stop => false
    }
    
    config[:start] # => true
    
    # Note that strings aren't the same as symbols
    
    config['stop'] # => nil

