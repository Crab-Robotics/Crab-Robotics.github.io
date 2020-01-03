---
width: full
navbar:
  sticky: true
  color: dark
  scroll_up: false
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: 1-1 # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_image: home-header-team.jpg
  background_align: center-center  
  background_overlay: "linear-gradient(to left top, rgba(82,229,231,0.8) 10%, rgba(47,47,162,0.9) 100%)"
  color: light
  height: full
  header_size: xlarge
  heading_size: large
  parallax: true
  container: small
  content:
    block: header-home
---

[comment]: # (This actually is the most platform independent comment)

{% if site.template == 'base' %}

  {% include cards.html 
    block="home-welcome" 
    section_size="large"
    section_title="Welcome To C.R.A.B. #39374"
    section_header_align="center"
    section_background="muted"
    section_content_align="center"
    section_padding_remove="bottom"
    card_style="primary"
    grid="1-4"
    gutter="small"
  %}

  {% include cards.html 
    block="home-outreach" 
    media="left" 
    section_size="large"
    section_padding_remove="bottom"
    section_background="muted"
    section_title="What We Do"
    section_header_align="center"
    card_style="default"
  %}

  {% include cards.html 
    block="home-corevalue" 
    media="right" 
    section_size="xsmall"
    section_padding_remove="bottom"
    section_background="muted"
    card_style="default"
  %}

  {% include cards.html 
    block="home-project" 
    media="left" 
    section_size="xsmall"
    section_background="muted"
    card_style="default"
  %}

  {% include cards.html 
    block="home-robot" 
    media="right" 
    section_size="large"
    section_padding_remove="top"
    section_background="muted"
    card_style="default"
  %}

  {% include cta.html
    block="home-current-year"
    layout="1"
    section_size="medium"
    section_content_align="center"
  %}

  {% include cta.html 
    section_size="large"
    section_background="#2F2FA2"
    section_container="small"
    section_content_align="center"
    section_content_color="light"
    layout="1"
    block="sponsors-partners"
  %}
  
{% else %}
{% endif %}