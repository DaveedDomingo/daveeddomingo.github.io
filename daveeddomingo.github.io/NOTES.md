Website is based on al-folio jekyll template:

https://github.com/alshedivat/al-folio

See CUSTOMIZE.md for more details on customization

Current base: 
  - v0.13.1
  - commit c5101beae4af04207ce99b55acb78f58983d4d2b
  - Date:   Thu Dec 12 16:23:28 2024 -0300

Some notes:
  - Website configuration in _config.yml
  - Can have larger than inline accountments, see example news template 2
  - Can disable/rearrange pages by modifying nav bool and nav order index
  - Modify how pages/posts are shown via liquid files in _layout

Other Notes on Changes:
  - disabled selected papers in about.md
  - disabled search in _config.yml
  - serve_og_meta enabled in _config.yml updated to profile pic
  - news title on about page changed to "recent news" in about.liquid:46
  - moved default news to _news_templates
  - Added cv viewer to _layouts/cv.liquid, can specify pdf file via cv_pdf in cv.md
  