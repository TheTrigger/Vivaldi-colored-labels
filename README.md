# Vivaldi Mail colored labels

I like the idea of Thunderbird Color Labels, but it is slow and often blocks, Vivaldi's email looks good, so finally I found a way to replicate it 😀

It could replate Thunderbird for daily work

## Setup

- Open `vivaldi://experiments`
- Enable `Allow for using CSS modifications`
- Open `Appearance` section in **settings**
- Choose the folder you want to use
  - `mkdir "%USERPROFILE%/Vivaldi"`
- Place your CSS files inside it (any name)

## Customize Labels

inside your `labels.css` or whatever

```css
/* single label tag */
#mail_view li[title='your_label'].MailLabels-Label { font-weight: bold; }

/* entire row with the label */
#mail_view div.tree-item:has(li[title='your_label']) { background: darkred; }
```

- Restart Vivaldi to see them in effect

# Taada!

## Other

Use `vivaldi://inspect/#apps` to inspect the view

You can add `javascript` scripts, see below



## Resources

- [`:has` selector](https://developer.mozilla.org/en-US/docs/Web/CSS/:has)
- [modding Vivaldi](https://forum.vivaldi.net/topic/10549/modding-vivaldi/)


## Donations

[paypal.me/trigger166](https://www.paypal.com/paypalme/trigger166)