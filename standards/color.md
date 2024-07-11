---
title: Color（色彩）

named:
  - name: Blue
    nameCn: 蓝色
    rgb: 
safe:
  - '00'
  - 33
  - 66
  - 99
  - CC
  - FF
---

```yml
white: FFFFFF
black: 000000
red:
yellow:
blue:
primary: 007bff 
info: 17a2b8 
success: 28a745 
warning: ffc107 
danger: dc3545 
dark: 343a40 
secondary: 6c757d 
light: f8f9fa 
```

- 天蓝色（Sky Blue）: RGB(135, 206, 235)
- 钢蓝色（Steel Blue）: RGB(70, 130, 180)
- 中蓝色（Medium Blue）: RGB(0, 0, 205)
- 绿宝石蓝（Turquoise Blue）: RGB(0, 199, 183)
- 夜空蓝（Midnight Blue）: RGB(25, 25, 112)

## 安全色（Safe Color）

<div class="row row-cols-6">

{% assign cor = page.safe %}
{% for r in cor %}
  {% for g in cor %}
    {% for b in cor %}
      <div class="col p-2">
        <div class="card" style="background:#{{r}}{{g}}{{b}}">
          <div class="card-body p-2">
            #{{r}}{{g}}{{b}}
          </div>
        </div>
      </div>
    {% endfor %}
  {% endfor %}
{% endfor %}
</div>
