<template>
  <div class="text-caption">
    <div v-for="i in paragraphAmt" :key="i">
      {{ paragraphs[i] }}
    </div>
  </div>
</template>

<script>
const paragraphs = ['Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Faucibus pulvinar elementum integer enim neque. Donec massa sapien faucibus et molestie ac. Tempor nec feugiat nisl pretium fusce id velit ut. Vitae sapien pellentesque habitant morbi tristique senectus et netus et. Nisi vitae suscipit tellus mauris a diam maecenas sed. Vestibulum lorem sed risus ultricies tristique nulla aliquet enim. Purus viverra accumsan in nisl nisi scelerisque eu. Commodo odio aenean sed adipiscing diam. Quam pellentesque nec nam aliquam sem et tortor consequat id. Nulla aliquet porttitor lacus luctus accumsan tortor. Fusce ut placerat orci nulla pellentesque dignissim. Varius vel pharetra vel turpis nunc. Orci porta non pulvinar neque laoreet suspendisse interdum. Amet consectetur adipiscing elit duis tristique sollicitudin nibh sit. In hac habitasse platea dictumst quisque sagittis purus sit amet.',

  'Vel turpis nunc eget lorem dolor sed viverra ipsum. Gravida arcu ac tortor dignissim convallis aenean et tortor at. Lobortis scelerisque fermentum dui faucibus in ornare quam viverra. Morbi tincidunt ornare massa eget egestas purus viverra accumsan in. Scelerisque in dictum non consectetur a erat nam at lectus. Euismod elementum nisi quis eleifend quam adipiscing. Volutpat consequat mauris nunc congue nisi vitae suscipit. Malesuada proin libero nunc consequat interdum varius sit amet. Id consectetur purus ut faucibus. Risus pretium quam vulputate dignissim suspendisse. Leo vel orci porta non pulvinar neque laoreet suspendisse. Massa placerat duis ultricies lacus sed. Ultricies integer quis auctor elit sed vulputate mi. Cursus mattis molestie a iaculis at erat pellentesque adipiscing commodo. Sit amet massa vitae tortor condimentum. Diam vel quam elementum pulvinar etiam non quam. Quam nulla porttitor massa id. Volutpat diam ut venenatis tellus in metus vulputate eu. Massa massa ultricies mi quis hendrerit dolor. Dui id ornare arcu odio ut sem.',

  'Aenean sed adipiscing diam donec adipiscing tristique. Egestas maecenas pharetra convallis posuere morbi leo urna. Sit amet massa vitae tortor condimentum lacinia. Placerat orci nulla pellentesque dignissim enim sit amet venenatis. Hac habitasse platea dictumst vestibulum rhoncus est. Placerat orci nulla pellentesque dignissim enim sit. Elit pellentesque habitant morbi tristique senectus. Phasellus egestas tellus rutrum tellus pellentesque eu tincidunt tortor aliquam. Vulputate odio ut enim blandit volutpat maecenas. Est ultricies integer quis auctor elit sed vulputate mi. Facilisi nullam vehicula ipsum a. Elementum tempus egestas sed sed risus. Risus quis varius quam quisque id diam vel. Euismod in pellentesque massa placerat. Est sit amet facilisis magna etiam tempor. Massa sapien faucibus et molestie ac. Libero nunc consequat interdum varius sit amet mattis vulputate enim. Nisi vitae suscipit tellus mauris a diam maecenas. Semper eget duis at tellus at urna condimentum mattis pellentesque.']

export default {
  data () {
    return {
      paragraphs,
      paragraphAmt: Math.floor(Math.random() * paragraphs.length)
    }
  }
}
</script>
