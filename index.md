## Most active GitHub users

This is a list of most active GitHub users in different countries/regions.
<ul class="country-list">
{% assign locations = site.data.locations | sort %}
{% for loc_hash in locations %}
  {% assign location = loc_hash[1] %}
  <li><a href="{{location.page | remove: '.html'}}">{{location.title}}</a></li>
{% endfor %}
</ul>

You can get a combined machine-readable JSON for:
<ul>
<li><a href="rank_only.json">rank-only with categories</a></li>
</ul>
A subset specific to each country/region is available on the individual page linked above.

### Badges

Badges are also available, which you can include on your profile pages. Simply include the following markdown for users:
```markdown
[![eplus.dev badge](https://user-badge.eplus.dev/REGION/USERNAME.svg)](https://user-badge.eplus.dev/REGION/USERNAME)
```
For organizations, you need to use a slightly different markup:
```markdown
[![eplus.dev badge](https://org-badge.eplus.dev/REGION/ORGNAME.svg)](https://org-badge.eplus.dev/REGION/ORGNAME)
```
In case you aren't currently ranked for a given region, you'll simply receive an "unranked" badge.
