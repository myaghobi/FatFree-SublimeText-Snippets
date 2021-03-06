# Fat-Free Framework SublimteText Snippets

Fat-Free Framework snippets for Sublime Text 4.


## INSTALLATION

Download and unzip the latest source from GitHub into your Sublime Text "Packages\User" directory and rename it to `FFSnippets`.

`Menu > Preferences > Browse Packages... > User`


## USAGE

`Menu > Preferences > Settings`

```json
{
    "tab_completion": true
}
```

| Trigger | Description |
| ------- | ----------- |
| Template |
| `ff@` | Fat-Free: {{ @var }} |
| `ffvar` | Fat-Free: {{ @var }} |
| `ffbaseurl` | Fat-Free: href="{{@BASE . '/' .@UI}}" |
| `ffcheck` | Fat-Free: &lt;check &gt;|
| `ffinclude` | Fat-Free: &lt;include &gt; |
| `ffisset` | Fat-Free: {{ isset(@var)?: }} |
| `ffloop` | Fat-Free: &lt;loop &gt; |
| `ffprintr` | Fat-Free: {{ print_r(@value) }} |
| `ffrepeat` | Fat-Free: &lt;repeat &gt; |
| `ffset` | Fat-Free: &lt;set > |
| `ffswitch` | Fat-Free: &lt;switch &gt; |
| `ffswitchcase` | Fat-Free: &lt;case &gt; |
| PHP |
| `ffbase` | Fat-Free: = \Base::instance() |
| `ffbase` | Fat-Free: = require('lib/base.php') |
| `ffaudit` | Fat-Free: \Audit::instance()-> |
| `ffauth` | Fat-Free: new \Auth(...) |
| `ffbase64` | Fat-Free: ->base64(...) |
| `ffclear` | Fat-Free: ->clear(...) |
| `ffcompile` | Fat-Free: ->compile(...) |
| `ffconcat` | Fat-Free: ->ffconcat(...) |
| `ffconfig` | Fat-Free: ->config(...) |
| `ffcopy` | Fat-Free: ->copy(...) |
| `ffcsv` | Fat-Free: ->csv(...) |
| `ffdevoid` | Fat-Free: ->devoid(...) |
| `ffdump` | Fat-Free: ->dump(...) |
| `fferror` | Fat-Free: ->error(...) |
| `ffexists` | Fat-Free: ->exists(...) |
| `ffflip` | Fat-Free: ->flip(...) |
| `ffget` | Fat-Free: ->get(...) |
| `ffhash` | Fat-Free: ->hash(...) |
| `ffmset` | Fat-Free: ->mset(...) |
| `ffmsetkey` | Fat-Free: 'key' => $value, |
| `ffnewjig` | Fat-Free: = new \DB\Jig(...) |
| `ffnewmongo` | Fat-Free: = new \DB\Mongo(...) |
| `ffnewsql` | Fat-Free: = new \DB\SQL(...) |
| `ffnewsqlite` | Fat-Free: = new \DB\SQL('sqlite:data/sqlite.db') |
| `ffpop` | Fat-Free: ->pop(...) |
| `ffpush` | Fat-Free: ->push(...) |
| `ffread` | Fat-Free: ->read(...) |
| `ffref` | Fat-Free: ->ref(...) |
| `ffrender` | Fat-Free: \Template->render |
| `ffreroute` | Fat-Free: ->reroute(...) |
| `ffroute` | Fat-Free: ->route(...) |
| `ffrun` | Fat-Free: ->run() |
| `ffscrub` | Fat-Free: ->scrub(...) |
| `ffserialize` | Fat-Free: ->serialize(...) |
| `ffsession` | Fat-Free: new \DB\SQL\Session(...) |
| `ffset` | Fat-Free: ->set(...) |
| `ffsign` | Fat-Free: ->sign(...) |
| `ffsplit` | Fat-Free: ->split(...) |
| `ffunserialize` | Fat-Free: ->unserialize(...) |
| `ffwrite` | Fat-Free: ->write(...) |

## CONFIGURATION

You can modify `ff-snippets-settings.tmPreferences` in your snippets (`Menu > Preferences > Browse Packages... > User > FFSnippets`):

```xml
<?xml version="1.0" encoding="UTF-8"?>
<plist version="1.0">
<dict>
    <key>name</key>
    <string>ff-snippets settings</string>
    <key>scope</key>
    <string>text.html.basic</string>
    <key>settings</key>
    <dict>
        <key>shellVariables</key>
        <array>
            <dict>
                <key>name</key>
                <string>FFSNIPPET_FATFREE_DEFAULT_TAG</string>
                <key>value</key>
                <string>f3</string>
            </dict>

            <!--
                Uncomment the following section if you like to opening brace not be formatted on a new line:
            -->
<!--             <dict>
                <key>name</key>
                <string>FFPHP_OPENING_BRACE</string>
                <key>value</key>
                <string>{</string>
            </dict> -->
        </array>
    </dict>
</dict>
</plist>
```
