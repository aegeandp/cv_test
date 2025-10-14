
# SDY60 CV Website (Jekyll + GitHub Pages)

Αυτό είναι starter για Jekyll site που κάνει deploy σε GitHub Pages με GitHub Actions (δεν χρειάζεται τοπική εγκατάσταση Ruby).

## Πώς προσθέτω άτομο
1. Πρόσθεσε νέα σελίδα στο φάκελο `bios/` με front matter:
   ```markdown
   ---
   layout: page
   title: <Ονοματεπώνυμο>
   permalink: /bios/<onoma-epwnymo>
   ---
   Περιεχόμενο...
   ```
2. Πρόσθεσε ένα entry στο `_data/people.yml`:
   ```yaml
   - name: <Ονοματεπώνυμο>
     url: /bios/<onoma-epwnymo>
   ```
3. Κάνε commit + Pull Request.

## Σημαντικό
- Το `baseurl` στο `_config.yml` είναι `/cv-website` γιατί είναι project site.
- Χρησιμοποίησε `{{ "/bios/..." | relative_url }}` για σωστά links.
