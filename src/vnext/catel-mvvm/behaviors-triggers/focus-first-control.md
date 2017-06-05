# FocusFirstControl

The Focus behavior is very powerful, but sometimes you just need to focus the first control on a window or control. This can be done by using the FocusFirstControl behavior instead. This behavior will focus the first control on a window or control and has only one property: *FocusParentFirst*.

Add the following XML namespaces:

``` {.java data-syntaxhighlighter-params="brush: java; gutter: false; theme: Confluence" data-theme="Confluence" style="brush: java; gutter: false; theme: Confluence"}
xmlns:i="clr-namespace:System.Windows.Interactivity;assembly=System.Windows.Interactivity"
xmlns:catel="http://catel.codeplex.com"
```

# Focus when the control is loaded

The easiest and default method is to focus the first control. The parent is also focused by default (just in case if it doesn't have any focus):

``` {.java data-syntaxhighlighter-params="brush: java; gutter: false; theme: Confluence" data-theme="Confluence" style="brush: java; gutter: false; theme: Confluence"}
<Window ...>
    <i:Interaction.Behaviors>
        <catel:FocusFirstControl />
    </i:Interaction.Behaviors>
</Window>
```