---
title: Weather
layout: default_notitle
city:
- name: Colorado Springs
  name_other: colorado-springs
  state: CO
- name: Troy
  name_other: troy
  state: MI
- name: Arlington
  name_other: arlington
  state: VA
- name: Phoenix
  name_other: phoenix
  state: AZ
---

# {{ page.title }}
<hr>
<a class="weatherwidget-io" href="https://forecast7.com/en/38d83n104d82/colorado-springs/?unit=us" data-label_1="Colorado Springs" data-label_2="CO" data-theme="pure" >Colorado Springs CO</a>
<script>
!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src='https://weatherwidget.io/js/widget.min.js';fjs.parentNode.insertBefore(js,fjs);}}(document,'script','weatherwidget-io-js');
</script>
<hr>
<a class="weatherwidget-io" href="https://forecast7.com/en/42d61n83d15/troy/?unit=us" data-label_1="Troy" data-label_2="MI" data-theme="pure" >Troy MI</a>
<script>
!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src='https://weatherwidget.io/js/widget.min.js';fjs.parentNode.insertBefore(js,fjs);}}(document,'script','weatherwidget-io-js');
</script>
<hr>
<a class="weatherwidget-io" href="https://forecast7.com/en/38d88n77d11/arlington/?unit=us" data-label_1="Arlington" data-label_2="VA" data-theme="pure" >Arlington VA</a>
<script>
!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src='https://weatherwidget.io/js/widget.min.js';fjs.parentNode.insertBefore(js,fjs);}}(document,'script','weatherwidget-io-js');
</script>
<hr>
<a class="weatherwidget-io" href="https://forecast7.com/en/33d45n112d07/phoenix/?unit=us" data-label_1="Phoenix" data-label_2="AZ" data-theme="pure" >Phoenix AZ</a>
<script>
!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src='https://weatherwidget.io/js/widget.min.js';fjs.parentNode.insertBefore(js,fjs);}}(document,'script','weatherwidget-io-js');
</script>
<hr>
<small>widget by <a href="https://weatherwidget.io">weatherwidget.io</a></small>

<!--
{% for item in page.city %}
<a class="weatherwidget-io" href="https://forecast7.com/en/38d83n104d82/{{ item.name_other }}/?unit=us" data-label_1="{{ item.name }}" data-label_2="{{ item.state }}" data-theme="pure" >{{ item.name }} {{ item.state }}</a>
<script>
!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src='https://weatherwidget.io/js/widget.min.js';fjs.parentNode.insertBefore(js,fjs);}}(document,'script','weatherwidget-io-js');
</script>
{% endfor %}
-->
