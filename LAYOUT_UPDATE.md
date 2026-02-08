# Layout Update Summary

The website layout has been completely redesigned to **exactly match** the original konstochansvar.se website structure.

## Changes Made

### 1. Layout Structure
- ✅ Changed from modern responsive layout to classic two-column fixed-width layout
- ✅ Container width: 780px (matching original)
- ✅ Body background: #DDDDDD (light gray)
- ✅ Container background: #FFFFFF (white) with 1px black border

### 2. Header
- ✅ Created `#bildhallare` div for logo image (780×128px)
- ✅ Removed modern header component
- ✅ Logo image path: `/assets/images/icons/ikalogo2.jpg`

### 3. Navigation
- ✅ Changed to table-based navigation matching original
- ✅ Navigation bar (`#navigationsfält`) with thin bottom border
- ✅ Links: Hem, Pressrum, Organigram, Vanliga frågor, Kontakt
- ✅ Font size: 12px
- ✅ Black text, underline on hover

### 4. Sidebar
- ✅ Left sidebar (`#sidebar1`) - 180px wide
- ✅ Contains project links (IKA Roundabout Art, etc.)
- ✅ Floated left with proper spacing
- ✅ Font size: 12px

### 5. Main Content
- ✅ Right column with `margin-left: 210px` (to account for sidebar)
- ✅ Content area with proper padding
- ✅ Images float left with `fltlft` class
- ✅ Font size: 12px
- ✅ Proper spacing for headings (h3, h5)

### 6. Footer
- ✅ Small footer with copyright
- ✅ Font size: 9px
- ✅ Margin-left: 210px (matching main content)
- ✅ Font: Arial, Helvetica, sans-serif

### 7. Typography & Colors
- ✅ Font family: Verdana, Arial, Helvetica, sans-serif
- ✅ Text color: #000000 (black)
- ✅ Links: Black, underline on hover
- ✅ Font sizes: 12px (main), 9px (footer)

### 8. CSS Classes
- ✅ `fltlft` - Float left (for images)
- ✅ `fltrt` - Float right
- ✅ `clearfloat` - Clear floats
- ✅ `style3` - Footer style
- ✅ `style5` - Blue text color (#0000FF)

## File Structure

### Updated Files
- `_layouts/default.html` - Complete redesign
- `_layouts/page.html` - Simplified
- `_layouts/home.html` - Simplified
- `_includes/navigation.html` - Table-based navigation
- `_includes/sidebar.html` - Sidebar component
- `assets/css/main.css` - Complete rewrite to match original
- `_data/navigation.yml` - Updated with correct pages
- `_data/sidebar.yml` - Created with sidebar items
- `_data/site.yml` - Updated site name to "IKA"
- `index.md` - Updated with homepage content structure

### Removed Files
- `_includes/header.html` - Not needed (logo in layout)
- `_includes/footer.html` - Not needed (footer in layout)

## Next Steps

1. **Add Logo Image**
   - Download `ikalogo2.jpg` (780×128px) from original site
   - Place in `assets/images/icons/ikalogo2.jpg`

2. **Add Content Images**
   - Download all images referenced in `index.md`
   - Place in `assets/images/content/`
   - See `ASSETS_NEEDED.md` for complete list

3. **Create Additional Pages**
   - Create pages for: pressrum.html, organigram.html, vanligafragor.html, kontakt.html
   - Create sidebar pages: roundaboutart.html, ebf.html, kidsclub.html, etc.

4. **Test Locally**
   ```bash
   bundle install
   bundle exec jekyll serve
   ```

5. **Verify Layout**
   - Check that layout matches original exactly
   - Verify all spacing and colors
   - Test on different screen sizes (responsive fallback included)

## Layout Specifications

- **Container**: 780px wide, centered, white background, 1px black border
- **Logo area**: 780×128px
- **Navigation**: Table with 5 columns, thin bottom border
- **Sidebar**: 180px wide, left-aligned
- **Main content**: Margin-left 210px, padding 20px
- **Footer**: Margin-left 210px, 9px font

## Responsive Behavior

A responsive fallback is included for screens smaller than 800px:
- Container becomes full-width
- Sidebar stacks above content
- Navigation table adapts

This maintains the original fixed-width design on desktop while providing basic mobile support.

