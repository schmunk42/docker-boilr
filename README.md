# boilr

:octocat: https://github.com/tmrts/boilr :whale: https://hub.docker.com/r/schmunk42/boilr/

## Installation

In your `.bashrc` add

    alias boilr="pwd | xargs -I {} -o docker run -it --rm -v ~/.config/boilr:/root/.config/boilr -v {}:/project --workdir /project schmunk42/boilr"
    
With the above alias you can use `boilr` as a command on your host, your current working directory is mapped to `/project` in the container.

## Example

```
cd my-project
boilr template download tmrts/boilr-license license
boilr template use license project-license
```

---

#### ![dmstr logo](http://t.phundament.com/dmstr-16-cropped.png) Built by [dmstr](http://diemeisterei.de)
