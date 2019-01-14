# Robotics Berlin Meetup

The Berlin Robotics Meetup is an informal meeting of robotics professionals and enthusiast in Berlin. We plan to hold it semi-regularly, roughly every two month at different locations announced here. We refrain from having formal talks, to lower the burden of preparation on the participants. It is more like a Stammtisch than a traditional meetup. We want to chat about the latest findings in your field of expertise, your problems of implementing that crazy IROS paper, or simply making fun on how every robot keeps on breaking every other day.
New (groups of) people are encouraged to introduce themselves and what they work on related to robotics with a short talk not longer than 5 minutes. You're not allowed to bring presentations, but you can either draw on a white board/flip chart or *bring your robot*.

What this is not:

* a recruiting event of any of the participating companies
* a forum to give introductory talks on robotics topics
* your way into robotics if you just heard it's the next big thing.

---
## News
{% for post in site.posts %}
  <article>
    <h3>
        {{ post.title }}
    </h3>
    <p>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time> &middot; by {{ post.user }}
    </p>
    {{ post.content }}
  </article>
{% endfor %}
