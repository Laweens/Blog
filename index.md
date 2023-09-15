Welcome to the start of Laweens journey in coding. 

![A photo of me](/assets/my_picture.jpe)

<ul>
    {% for post in site.posts %}
    <li>
     <a href="{{ post.url }}"> {{ post.title }}</a>
    </li>
    {% endfor %}
</ul>