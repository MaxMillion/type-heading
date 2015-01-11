---
category: heading
title: th-heading
description: Return a heading list.
format: th-heading-get-map($heading)
params: [
  foo: [
    ret: 'mixed',
    desc: 'A mixed value.',
    req: 'Yes',
    def: '10px',
    cont: '$var'
  ],
  bar: [
    ret: 'string',
    desc: 'A string value.',
    req: 'No',
    def: false,
    cont: false
  ]
]
---
With heading map key:

{% highlight sass %}
// Set heading property values
$th-headings: ( h1: (36px 42px 20px, 42px 48px 20px 768px) );

// Output: 36px 42px 20px
@debug th-heading-get(h1);
{% endhighlight %}

With heading map key and heading list breakpoint:

{% highlight sass %}
// Set heading property values
$th-headings: ( h1: (36px 42px 20px, 42px 48px 20px 768px) );

// Output: 42px 48px 20px 768px
@debug th-heading-get(h1, 768px); 
{% endhighlight %}