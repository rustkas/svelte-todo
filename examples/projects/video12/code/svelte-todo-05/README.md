# <svelte:component>

`<svelte:component>` позволяет отрисовать компонент динамически, когда заранее неизвестно какой компонент нужно отрисовать.
При этом хотелось бы избежать многочиселнных блоков `{#if} ... {:else}` в разметке.

`<svelte:component>` может быть полезен для реализации такого компонента, как, например, `Tabs`.
