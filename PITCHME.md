
#HSLIDE

# LESS Training 2/23/16

#HSLIDE

# Reflecting Markup via nesting
        html:
        <div id="container-box">
          <span class="inside-box">
            <strong>This is a strong sentence.</strong>
          </span>
        </div>

        less:
        #container-box {
          .inside-box {
            > strong { color: @blue; }
          }
        }

<div class="example-box">
  <div id="container-box">
    <span class="inside-box">
      <strong>This is a strong sentence.</strong>
    </span>
  </div>
</div>

#HSLIDE

# Media Queries

#HSLIDE

# Imports

#HSLIDE

# Variables
  * Color Variables
        @black: #000;
        @white: #fff;
  * Fonts
        @import url('https://fonts.googleapis.com/css?family=Roboto|Slabo+27px');
        @sans: 'Roboto';
        @serif: 'Slabo';
#HSLIDE
# Mixins
  * Color change
  * Font Cycle
  * Animation
#HSLIDE

# DealerSpike Specific Functionality

#HSLIDE

# Theme Folder Structure
        |-less/
        |---themes/
        |-----dealershipname/
        |-------stylers/
        |---------button-styler.less
        |---------calendar-styler.less
        |---------carousel-styler.less
        |---------footer-styler.less
        |---------general-styler.less
        |---------inventory-styler.less
        |---------navbar-styler.less
        |---------social-button-styler.less
        |-------footer.less
        |-------header.less
        |-------main-home.less
        |-------styler.less
        |-------theme.less
        |-------variables.less
        |---custom.less
        |---promos.less

#HSLIDE

# DS-specific Mixins

#HSLIDE

# Mockup Theme Changes

#HSLIDE

### Materials
- FED breakdown sheet with sizes and whatnot
