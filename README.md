## Network

[HAR](./www.gd.ru.har)

Неоптимальные места:

- Дублирование ресурсов
  - Bootsrtap и Popper загружаются дважды: они включены в bootstrap.bundle.min.js
    ![bootstrap in network tab](/images/bootstrap_network.png)
    ![popper in network tab](/images/popper_network.png)
    ![bootstrap in source code](/images/bootstrap_source.png)
    ![bootstrap docs](/images/bootstrap_docs.png)

  - code.js загружается дважды
  ![code.js](/images/code_js_network.png)

  - Повторная загрузка шрифта
    ![font-awesome](/images/font_awasome_network.png)
  
  - openapi.js
    ![openapi.js](/images/openapi_js_network.png)

## Performance

[Профиль загрузки](./performance_profile.json)

Время до:
- FP (first paint) - 649ms
- FCP (first contentful paint) - 649ms
- DCL (DOM content loaded) - 2010ms
- LCP (largest contentful paint) - 2520ms
- Load - 11690ms

DOM-элемент с LCP:
![dom-element with lcp](/images/lcp.png)

Затраченное время на разные этапы обработки документа:
- Loading: 40ms
- Scripting: 1861ms
- Rendering: 715ms
- Painting: 95ms

![performance chart](/images/perf_chart.png)

## Coverage

![coverage](/images/coverage.png)

Объём неиспользованного CSS: 558kB
Объём неиспользованного JS: 2020kB
