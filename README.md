# Seven languages in 90 minutes

Is it possible to show 7 languages in a 90 minutes presentation? In this session, I will give that a try.

## Presentation
I'm below average when it comes to typing. When typing in front of an audience, it's even worse.

Since I don't want to bore my audience, I'm going to use git commits as slides. For this, I'm introducing two new git aliases:
`git next` and `git prev`.

To start the presentation: `git checkout demo-start`
To move to the next step : `git next`
To move one step back    : `git prev`

To configure these aliases, run these scripts:
git config --global alias.next '!git checkout `git rev-list HEAD..master | tail -1`'
git config --global alias.prev 'checkout HEAD^'

Source: http://www.jayway.com/2015/03/30/using-git-commits-to-drive-a-live-coding-session/
