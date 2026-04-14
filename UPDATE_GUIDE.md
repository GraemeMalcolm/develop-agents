# Updating from Template

If you created a repository from this template before the latest fixes, follow these steps:

## Required Changes

1. **Create the module data file** - Create `_data/module.yml` with your module information:

   ```yaml
   title: "Your Module Title"
   description: "Your module description."
   level: 200
   ```

2. **Update _config.yml** - Make sure it excludes README.md:

   ```yaml
   exclude:
     - spec.md
     - README.md
     - Gemfile
     - Gemfile.lock
   ```

3. **Replace _includes/navigation.html** - Copy the latest version from the template (fixes navigation spacing).

4. **Update _layouts/content.html** - Ensure it uses `{{ site.data.module.title }}` instead of README frontmatter.

5. **Update index.md** - Ensure it uses `{{ site.data.module.title }}` instead of README frontmatter.

## Verify

After pushing changes:

- Landing page should show module title, level, and description
- Content pages should show module title as H1 (linked to home)
- Previous/Next buttons should be centered
- Navigation should work correctly

## Clear Cache

If changes don't appear immediately:

1. Wait 1-2 minutes for GitHub Pages to rebuild
2. Clear your browser cache
3. Try accessing in an incognito window
