# Use eLuvLetter

[![license](https://img.shields.io/github/license/george-chou/eLuvLetter.svg)](https://github.com/george-chou/eLuvLetter/blob/master/LICENSE)
[![Deploy static content to Pages](https://github.com/george-chou/eLuvLetter/actions/workflows/static.yml/badge.svg?branch=main)](https://github.com/george-chou/eLuvLetter/actions/workflows/static.yml)

## Important links
|    Name    | URL                                          |
| :--------: | :------------------------------------------- |
|    Git     | <https://git-scm.com/downloads>              |
|   GitHub   | <https://github.com>                         |
| eLuvLetter | <https://github.com/george-chou/eLuvLetter>  |
|  Netlify   | <https://app.netlify.com>                    |
|  2D Demo   | <https://eluvletter.pages.dev>               |
|  3D Demo   | <https://eluvletter.pages.dev/index-3d.html> |

Note: the heartbeat animation indicates that the BGM is loading, please be patient and wait.

## Customize

0. Download and install Git;

1. Register a GitHub account, set SSH, and fork a copy of this repository to your own account;

2. Clone the repository to local:
```
git clone https://github.com/%Your_GitHub_Account%/eLuvLetter.git
```

3. Go to the `./eLuvLetter/font/` directory, open `content.json`, and customize the configuration as follows:

```
{
    "to"        : "envelope recipient",
    "from"      : "sign",
    "recipient" : "letter recipient",
    "title"     : "Web page tab title",
    "stamp"     : "Stamp URL",
    "bgm"       : "BGM URL",
    "text"      : "letter ^n content"
}
```

The symbol `^n` in the demo means that the typewriter pauses for n milliseconds,

BGM URL is the default mp3 directory or mp3 direct link in the demo code(Note: It is best not to use the API to get mp3, it may be blocked by cross-domain)

If you use the default directory, you can rename your mp3 to `bgm.mp3` and overwrite `bgm.mp3` under `./eLuvLetter/bgm` to achieve custom modification of BGM

## Deploy to Netlify
1. Sync the modified local code to your GitHub account:
```
cd eLuvLetter
git add .
git commit -a
# i
# input description
# :wq!
git push
```
2. Enter [Netlify official website](https://app.netlify.com);
3. Use your GitHub account to login by authorization, click `Add new site` - `Import an existing project`;
4. Click `GitHub`, enter the keyword `eLuvLetter` in the search box to find the previously forked repo, and select it;
5. Click `Deploy site` to jump into `Site overview` page automatically, click `Site settings`;
6. Click `Change site name` under `Site information`, modify second-level domain name not conflict to others, and click `Save`;
7. After the deployment, we can visit `https://%PROJECT_NAME%.netlify.app` to broswe your page(The `%PROJECT_NAME%` is the second-level domain name customized just now)

*Good luck!*
