# Active Record is indeed magical

We know that MiniTest runs tests in random order. However did you know
that all the tests in Active Record run in a sorted order?

Do you know the difference between `CollectionProxy` and `Relation` ? Do you know why in a has_many through case `@physician.patients.create!` would work but `@physician.patients.where(active: true).create!` would silently fail without creating the association record?

Active Record has not one but three save methods. How all these three
save methods work together.

There is something magical when you do `User.where(id: '20')`. Can you
spot it ?

In Rails 3 when where conditions are merged then the last where condition wins. In Rails 4 all the where conditions are 'And'ed. But not defautl_scope. We will see how and why.

Do you know all the edge cases related to `inverse_of` ?

This talk will answer all those questions and a more magics that Active
Record brings us and we will see why all those magics are good for us.

## Neeraj Singh

Neeraj loves Ruby, JavaScript and open source culture. He has done extensive contribution to Ruby on Rails framework primarily in the Active Record area. He is a core contributor to Rails's jquery-ujs library.

He has contributed to many open source applications including ActiveMerchant, Spree and jQuery. He has written extensively about inner workings on Ruby on Rails and jQuery at his [Blog](http://blog.bigbinary.com). He runs [BigBinary](http://bigbinary.com) where he primarily uses RubyOnRails and RubyMotion.

![Profile picture](http://bigbinary.com/assets/team/neeraj.jpg)

- [My website](http://BigBinary.com)
- [My twitter](https://twitter.com/neerajdotname)
- [Past talk slides](https://speakerdeck.com/neerajdotname)
- [Past talk video](http://confreaks.com/videos/2729-wickedgoodruby-activerecord-is-still-magical)
