#  Модули

Модули позволяют иметь общий код или состояние между компонентами, например между всеми экземплярами одного и того же компонента.

Бывает полезно запустить один и тот же код для всех экземпляров компонента.

Модуль это тег `<script>`, который имеет значение свойства `context="module"`.

```
<script context="module">

</script>
```

Данный участок кода выполняется только один раз ещё до создания какого-либо компонента, а не при каждой инициализации экземпляра компонента.

Переменные, которые объявлены в блоке `context="module"` могут быть использованы, как в коде, так и в разметке. Данные переменные не являются реативными. Т.е. присваивание этим переменным новых значений не будут приводить к перерисовке данного компонента.

## Типы переменных и их особенности

### script module 
не реактивные
доступны между экземплярами одного и того же компонента

### store
реактивные
доступны во всём приложении

### context
не реактивные
доступны в компоненте и его потомках

