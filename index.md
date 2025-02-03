---
layout: page
title: Home / Schedule
nav_order: 1
description: A week-to-week description of the content covered in the course.
course:
  edstem: https://edstem.org/us/courses/74189
  faq: https://ds100.org/faqs/sp25
currWeekNumber: 3
---

# Data 100: Principles and Techniques of Data Science

{: .mb-2 }
UC Berkeley, Spring 2025
{: .mb-0 .fs-6 .text-grey-dk-000 }

[Ed](https://edstem.org/us/courses/74189){:target="\_blank" .btn .btn-ed .mr-1 }
[Datahub](http://data100.datahub.berkeley.edu/){:target="\_blank" .btn .btn-datahub .mr-1 }
[Gradescope](https://www.gradescope.com/courses/949942){:target="\_blank" .btn .btn-gradescope .mr-1 }
[Lectures Playlist](https://youtube.com/playlist?list=PLQCcNQgUcDfqdZpmNOM4VYwloa2TFQYQf&si=ZPtsLCOyuzQ_HMM_){:target="\_blank" .btn .btn-youtube .mr-1}
[Additional Accommodations](https://docs.google.com/forms/d/e/1FAIpQLSe23BU7DocByEPYt6YV00rOTn7K1AVj7Fqpw2eOgWG0Q5GtDw/viewform?usp=sharing){:target="\_blank" .btn .btn-blue .mr-1 }
[Office Hours Queue](https://oh.ds100.org/){:target="\_blank" .btn .btn-oh .mr-1}

<div>
{% assign instructors = site.staffers | where: 'role', 'Instructor' | sort: 'order' %}
  <div class="role">
    {% for staffer in instructors %}
    <!-- {% assign staffer.photo = staffer.photo | replace: '../', '' %} -->
    {{ staffer }}
    {% endfor %}
  </div>
</div>

{: .highlight }

> Welcome to [Week {{page.currWeekNumber}}](#week-{{page.currWeekNumber}}) of Data 100!
> 
> Lectures will be webcast at: [https://berkeley.zoom.us/j/97347722542](https://berkeley.zoom.us/j/97347722542){:target="\_blank"}.


<!-- {: .note }
> <span style="color:red">**Enrollment: As of Jan. 23, 2024, Data C100/200 is closed and no further enrollment is possible.**</span>  -->


<a name="schedule"></a>

## Schedule

{% for module in site.modules %}
{{ module }}
{% endfor %}