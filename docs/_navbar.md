- **Translations**
    - [:ru: Russian](/ru-RU/)
    - [:us: English](/en-US/)

<li>
  <p><strong>Color themes</strong></p>
  <ul class="theme-preview">
    <li>
      <a class="active"><img class="emoji" src="https://github.githubassets.com/images/icons/emoji/sun_with_face.png" alt="sun_with_face" data-theme="vue"> Light</a>
    </li>
    <li>
      <a><img class="emoji" src="https://github.githubassets.com/images/icons/emoji/new_moon_with_face.png" alt="new_moon_with_face" data-theme="dark"> Dark</a>
    </li>
    <li>
      <a><img class="emoji" src="https://github.githubassets.com/images/icons/emoji/art.png" alt="art" data-theme="pure"> Simple</a>
    </li>
  </ul>
</li>

<style>
  .theme-preview a:hover {
    cursor: pointer;
    text-decoration: underline;
  }  
</style>

<script>
  var preview = Docsify.dom.find('.theme-preview');
  var themes = Docsify.dom.findAll('[rel="stylesheet"]');

  preview.onclick = function (e) {
    var title = e.target.getAttribute('data-theme')

    themes.forEach(function (theme) {
      theme.disabled = theme.title !== title
    });
  };
</script>