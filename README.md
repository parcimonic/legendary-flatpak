# legendary-flatpak

## Archival notice

I'm not actively working on this project and have no plans to update it in the foreseeable future.

---

This is an *unnoficial* version of [legendary](https://github.com/derrod/legendary) built with Flatpak.

I'm doing this just to learn more about Flatpak and obviously to use the sandbox for games. Inspired by [Steam](https://github.com/flathub/com.valvesoftware.Steam) and [Bottles](https://github.com/flathub/com.usebottles.bottles).

## Unnoficial status

Please *do not report* bugs or issues with this version of legendary to the main author's repository, unless we've discussed it in the issue tracker and agreed to submit it upstream. This Flatpak package is unnoficial, not supported/backed/approved by derrod in any way, it may (or may not) have issues that are not present in the upstream version.

If/when this project is more mature, I'll contact derrod and check if we can make this an official supported package.

## Building

If you've never done this before, please follow the the [documentation](https://docs.flatpak.org/en/latest/first-build.html#test-the-build) up to step 5. This will set you up with all current pre-requirements for this project and (hopefully) give you a bit of understanding about building flatpaks.

Then you can run `flatpak-builder --user --install --force-clean build-dir com.gitlab.parcimonic.legendary.yml` to build and install this package.

Run it with `flatpak run com.gitlab.parcimonic.legendary`. Use `flatpak run --command=bash com.gitlab.parcimonic.legendary` to open a bash shell in the sandbox.

## Installing

You can get the GitLab build artifacts [here](https://gitlab.com/parcimonic/legendary-flatpak/-/jobs), then install using `flatpak install legendary.flatpak`.

## Contributing

When submitting changes to the Flatpak manifest, please try to be as descriptive as possible, since the plan here is to learn more about Flatpak.

I'm trying to not rely on pre-build binaries, so please have this in mind when adding new code to the Flatpak package.

Helpful links:

- [Flatpak docs](https://docs.flatpak.org/en/latest/building.html)

- [Builder tools](https://github.com/flatpak/flatpak-builder-tools)
