<template>
  <div> 
    <NuxtLayout> <!-- To apply the layout (layouts/default.vue) to all pages, we need to wrap the content of the page in a <NuxtLayout> component. This component will render the layout and the page content.-->
      <NuxtPage /> <!-- The <NuxtPage> component is a special component that will render the page content. -->
    </NuxtLayout>
  </div>
</template>
