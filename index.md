# Berlin Robotics Meetup

*Next meetup:* <a href="#news-1">30th March 2023, 6:30 pm, at the Micropsi Industries office</a>

The Berlin Robotics Meetup is an informal meeting of robotics professionals and enthusiasts from academia and industry in Berlin. This event enables us to build a robotics community in Berlin to network and share insights.

We plan to hold it regularly, roughly every two months, at different locations announced here, on meetup.com and LinkedIn.

What do we want to do here?
We want to chat about the findings in your field of expertise, your problems with implementing that crazy IROS paper, make fun of how every robot keeps breaking every other day, sharing the best practices and pitfalls of a robotic business.

---
## News
{% for post in site.posts %}
  <article>
    <h3 id="news-{{ forloop.index }}">
       {{ post.title }}
    </h3>
    <p>
    <small>posted at <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time> &middot; by {{ post.user }}</small>
    </p>
    {{ post.content }}
  </article>
{% endfor %}
