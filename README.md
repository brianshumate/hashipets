# hashipets

    --------------------------------------------
    ============================================
     _               _     _            _
    | |__   __ _ ___| |__ (_)_ __   ___| |_ ___
    | '_ \ / _` / __| '_ \| | '_ \ / _ \ __/ __|
    | | | | (_| \__ \ | | | | |_) |  __/ |_\__ \
    |_| |_|\__,_|___/_| |_|_| .__/ \___|\__|___/
                            |_|

    ============================================
    --------------------------------------------

## What?


**hashipets** is a collection of CLI snippets for use with HashiCorp tools like
[Consul](https://www.consul.io/), [Nomad](https://www.nomadproject.io/), [Packer](https://www.packer.io/), [Terraform](https://www.terraform.io/), [Vagrant](https://www.vagrantup.com/), and [Vault](https://www.vaultproject.io/).

The snippets are kept in a TOML formatted file that is compatible with the simple command-line snippet manager [pet](https://github.com/knqyf263/pet).

> **NOTE**: The commands in `hashipets.toml` should reflect those available in recent versions of the tool they apply to.

## Why?

It's a tool and workflow for recalling and sharing complex CLI one-liners and seldom used but otherwise useful command line invocations.

## How?

Using the fantastic CLI utility `pet` and the [hashipets.toml](https://github.com/brianshumate/hashipets/blob/master/hashipets.toml) in this repository, you'll be commanding HashiCorp tools like a pro in no time!

### Quick Start for macOS

0. Clone this repository within some `$DIR`
1. Install `pet`: `brew install knqyf263/pet/pet`
2. Configure: `pet configure`
3. Point `snippetfile` to `$DIR/hashipets/hashipets.toml`, save, and exit
4. 🎉

### What's Next?

You can optionally customize the `peco` fuzzy finder tool like so:

```
$ mkdir $HOME/.config/peco && \
  cp $DIR/hashipets/peco_config.json $_/config.json
```

Then use `pet` in awesome ways:

#### List all snippets

```
$ pet list
```

#### Search snippets

```
$ pet search
```

#### Add search result to clipboard on macOS

```
$ pet search | pbcopy
```

#### Execute a snippet

```
$ pet exec
```

#### Interactively add a snippet

```
$ pet new
Command> curl -s <consul_http_addr>/v1/status/peers
Description> Get Consul server peers from HTTP API
```

See the [pet documentation](https://github.com/knqyf263/pet/blob/master/README.md) for more ways to use it!

## Resources

Here are some links to resources for the technologies used in this project:

- [Consul](https://www.consul.io/)
- [Nomad](https://www.nomadproject.io/)
- [Packer](https://www.packer.io/)
- [Terraform](https://www.terraform.io/)
- [Vagrant](https://www.vagrantup.com/)
- [Vault](https://www.vaultproject.io/)
- [pet](https://github.com/knqyf263/pet)
- [fzf](https://github.com/junegunn/fzf)

## Who?

**hashipets** was created by [Brian Shumate](https://github.com/brianshumate) and made possible through the generous time of the good people named in [CONTRIBUTORS.md](https://github.com/brianshumate/hashipets/blob/master/CONTRIBUTORS.md)

## Special Thanks

Thanks to **[Teppei Fukuda](https://github.com/knqyf263)** for making `pet`!
