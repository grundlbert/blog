---
title: Wallabys!
bg_img: /main_img/NEUSEELAND.JPG
layout: bonuspage
---

## Wilkommen auf der Wallaby-Bonusseite!

#### Hier gibt vor allem (aber nicht ausschließlich) Fotos von Wallabys! Viel Spaß damit :D

{% include image.html file="/14roadtrip1/07-07.JPG" description="Wallabies mögen Martin" width="85%" %}
{% include image.html file="/14roadtrip1/07-09.JPG" description="Martin und Wallabies!" width="85%" %}
{% include image.html file="/14roadtrip1/07-10.JPG" description="Wallabie!" width="85%" %}
{% include image.html file="/14roadtrip1/07-11.JPG" description="Wallabie!" width="85%" %}
{% include image.html file="/14roadtrip1/07-12.JPG" description="Martin mit noch mehr Wallabies" width="85%" %}
{% include image.html file="/14roadtrip1/07-13.JPG" description="Ein Wallabie findet die Kamera spannend" width="85%" %}
{% include image.html file="/14roadtrip1/07-14.JPG" description="Wallabie!" width="85%" %}
{% include image.html file="/14roadtrip1/07-15.JPG" description="Wallabie!" width="85%" %}
{% include image.html file="/14roadtrip1/07-16.JPG" description="Martin!" width="85%" %}
{% include image.html file="/14roadtrip1/07-17.JPG" description="Martin und Wallabie!" width="85%" %}
{% include image.html file="/14roadtrip1/07-18.JPG" description="Pfau!" width="85%" %}
{% include image.html file="/14roadtrip1/07-19.JPG" description="Daliah und Wallabie!" width="85%" %}
{% include image.html file="/14roadtrip1/07-20.JPG" description="Wallabie mit kleiner süßer Zunge!" width="85%" %}
{% include image.html file="/14roadtrip1/07-21.JPG" description="Gieriges Wallabie" width="85%" %}
{% include image.html file="/14roadtrip1/07-22.JPG" description="Pfau!" width="85%" %}
{% include image.html file="/14roadtrip1/07-23.JPG" description="Daliah mit zwei Wallabies!" width="85%" %}
{% include image.html file="/14roadtrip1/07-24.JPG" description="Daliah mit zwei Wallabies!" width="85%" %}
{% include image.html file="/14roadtrip1/07-25.JPG" description="Die Dame, der die Wallabiefarm gehört, hat auch einen kleinen Hund, der gerne Ohren frisst..." width="85%" %}

<div class="textbox1">
    <center>
        <a href="/2023/02/14/roadtrip.html">Ich will zurück zum Blogeitrag!</a>
    </center>
</div><div class="com_Section">
    <form id="postCommentFormNetlify" method="POST" netlify-honeypot="bot-field" data-netlify="true" accept-charset="utf-8">
        <h2>Kommentare</h2>
        <input type="hidden" name="subject" value="Blog Kommentar" /><br><br>
        <input type="hidden" name="blogpost" value="{{ page.title }}" />
        <label>Name:<br><input type="text" name="name" placeholder="Dein Name" required></label><br><br>
        <label>Gib deinen Senf dazu!<br><textarea name="message" placeholder="Deine Nachricht"></textarea></label><br>

        <!--<label>Mein Kommentar soll veröffentlicht werden:</label>
            <input type="checkbox" name="veroeffentlichen" value="yes" checked><br><br> -->
        <i>
            <label>
                <br>Da die Kommentare für uns der einzige Weg sind herauszufinden wer das eigentlich so liest was wir so schreiben freuen wir uns vollgas über jeden Einzelnen! :D
                <br>Jeder Kommentar wird von uns hochqualitativ und eigenhändig eingefügt wird, deshalb kann es ein Bisschen dauern, bis er hier erscheint.<br>
                <br>Alle Kommentare werden veröffentlicht.<br
            </label>
        </i><br>
        <div class="cell">
            <button type="submit" class="button" name="submit">Abschicken</button>
        </div> 
    </form>
    <br>
    
    {% for item in site.data.comments %}
        {% if item.post == page.comment_title %}
            <div class="com_Comment">
                <h5>{{ item.date }} - {{ item.name }}</h5>
                {% capture postcomment %}{% include comments/{{ item.message }} %}{% endcapture %}
                {{ postcomment | markdownify }}
            </div>
        {% endif %}
    {% endfor %}
</div>