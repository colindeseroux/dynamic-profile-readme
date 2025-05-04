# Dynamic profile README

The purpose of this project is just to document how my profile README works.

## Stats

These stats come from 2 different repositories.

The first statistics come from [github-readme-stats](https://github.com/anuraghazra/github-readme-stats).<br />
To include commits in private repositories you can either host it with your [PAT token](https://github.com/colindeseroux/github-readme-stats#deploy-on-your-own) with vercel or under [Docker](https://github.com/colindeseroux/github-readme-stats#on-docker-platform).

```html
<img
  alt="Phenix333's Github Stats"
  height="230px"
  src="https://github-stats.colindeseroux.fr/?username=Colin-de-Seroux&amp;locale=en&amp;theme=tokyonight&amp;rank_icon=github&amp;border_color=2e4058"
/>
```

<img alt="Phenix333's Github Stats" height="230px" src="https://github-stats.colindeseroux.fr/?username=Colin-de-Seroux&amp;locale=en&amp;theme=tokyonight&amp;rank_icon=github&amp;border_color=2e4058"/>

```html
<img
  alt="Phenix333's Language Stats"
  height="600px"
  src="https://github-stats.colindeseroux.fr/top-langs?username=Colin-de-Seroux&amp;langs_count=100&amp;exclude_repo=S5-AR&amp;hide=makefile,blade,purebasic,cmake,perl,llvm,rust,hack,ruby,objective-c,batchfile,jupyter%20notebook&amp;layout=donut&amp;local=en&amp;theme=tokyonight&amp;border_color=2e4058"
/>
```

<img alt="Phenix333's Language Stats" height="600px" src="https://github-stats.colindeseroux.fr/top-langs?username=Colin-de-Seroux&amp;langs_count=100&amp;exclude_repo=S5-AR&amp;hide=makefile,blade,purebasic,cmake,perl,llvm,rust,hack,ruby,objective-c,batchfile,jupyter%20notebook&amp;layout=donut&amp;local=en&amp;theme=tokyonight&amp;border_color=2e4058"/>

The second statistics come from [github-readme-streak-stats](https://github.com/DenverCoder1/github-readme-streak-stats).<br />
To include contributions in private repositories, turn on the setting for "Private contributions" from the dropdown menu above the contribution graph on your profile page.

```html
<img
  alt="Phenix333's Github Stats 2"
  height="210px"
  src="https://streak-stats.demolab.com/?user=Colin-de-Seroux&amp;theme=tokyonight-duo&amp;border=2E4058&amp;background=1A1B27"
/>
```

<img alt="Phenix333's Github Stats 2" height="210px" src="https://streak-stats.demolab.com/?user=Colin-de-Seroux&amp;theme=tokyonight-duo&amp;border=2E4058&amp;background=1A1B27"/>

## Repos

I've set up a github action to retrieve all the public projects I've committed to and automatically add them to my README as soon as I create a new project, participate in an existing project or make an existing project public. The cron is triggered every hour.

To automatically retrieve all the projects you have worked on:

- simply add this div tag `<div id="repos"></div>` to your README.
- copy `update-readme-repos.yml` in `.github/workflows/`.
- create a second PAT token with `repo` and `read:org`.
- in repository `Settings -> Secrets and variables -> Actions -> Secrets -> New repository secret` name **GH_TOKEN**.
- in repository `Settings -> Secrets and variables -> Actions -> Variables -> New repository variable` name **EXCLUDED_REPOS** with the rest you don't want to see (Ex: Colin-de-Seroux/test,Colin-deSeroux/Colin-de-Seroux).

```html
<div id="repos"></div>
```

<div id="repos">
    <a href="https://github.com/Colin-de-Seroux/Projet_developpement_logiciel_application_IA_embarquee">
        <img alt="Projet_developpement_logiciel_application_IA_embarquee" src="https://github-stats.colindeseroux.fr/pin/?username=Colin-de-Seroux&amp;repo=Projet_developpement_logiciel_application_IA_embarquee&amp;theme=tokyonight&amp;border_color=2e4058"/>
    </a>
    <a href="https://github.com/Pierrad/InstaDAM">
        <img alt="InstaDAM" src="https://github-stats.colindeseroux.fr/pin/?username=Pierrad&amp;repo=InstaDAM&amp;theme=tokyonight&amp;border_color=2e4058"/>
    </a>
    <a href="https://github.com/H4znow/marioBrossGame">
        <img alt="marioBrossGame" src="https://github-stats.colindeseroux.fr/pin/?username=H4znow&amp;repo=marioBrossGame&amp;theme=tokyonight&amp;border_color=2e4058"/>
    </a>
</div>
