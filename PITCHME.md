# LESS Training 2/23/17

#HSLIDE

### Reflecting Markup via nesting

#VSLIDE

html:

        <div id="container-box-1">
          <span class="inside-box">
            <strong>This is a strong sentence.</strong>
          </span>
        </div>
less:

        #container-box-1 {
          .inside-box {
            > strong { color: @blue; }
          }
        }
result:

<div class="example-box">
  <div id="container-box-1">
    <span class="inside-box">
      <strong>This is a strong sentence.</strong>
    </span>
  </div>
</div>

#HSLIDE

### Media Queries

#VSLIDE

    .container {
      .inner-container {
        .inner-box {
          font-size: 12px
          @media(min-width: @sm-min) {
            font-size: 16px;
          }
        }
      }
    }

#VSLIDE

        .container {
          .inner-container {
            .inner-box {
              font-size: 12px
            }                        
          }
          @media(min-width: @sm-min) {
            .inner-container {
              .inner-box {
                font-size: 16px;        
              }
            }
          }
        }

#HSLIDE

### Variables/Imports
colors:

        @black: #000;
        @white: #fff;
fonts:

        @import url('https://fonts.googleapis.com/css?family=Roboto|Slabo+27px');
        @sans: 'Roboto';
        @serif: 'Slabo';
#HSLIDE
### Mixins
* Color change
* Animation
#HSLIDE

# DealerSpike Specific Functionality

#HSLIDE

### Theme Folder Structure
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

### DS-specific Mixins

#HSLIDE

### END
