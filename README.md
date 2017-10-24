# hashipets

    --------------------------------------------
    ============================================
     _               _     _            _
    | |__   __ _ ___| |__ (_)_ __   ___| |_ ___
    | '_ \ / _` / __| '_ \| | '_ \ / _ \ __/ __|
    | | | | (_| \__ \ | | | | |_) |  __/ |_\__ \
    |_| |_|\__,_|___/_| |_|_| .__/ \___|\__|___/
                            |_|

    [[[[[[[[[[[[[[[[[[[[[[]]]]]]]]]]]]]]]]]]]]]]

## What?

**hashipets** is a collection of snippets for use with HashiCorp tools like
Consul, Nomad, Packer, Terraform, Vagrant, and Vault. The snippets are kept in a TOML file that is compatible with the simple command-line snippet manager [pet](https://github.com/knqyf263/pet).

## Why?

It's a nice means of recalling and sharing complex one-liners and seldom used commands.

## How?

Using the fantastic CLI utility `pet` and the [hashipets.toml] in this repository, you'll be comanding HashiCorp tools like a pro in no time!

### Quick Start for macOS

0. Clone this repository within some `$DIR`
1. Install `pet`: `brew install knqyf263/pet/pet`
2. Configure: `pet configure`
3. Point `snippetfile` to `$DIR/hashipets/hashipets.toml`, save, and exit
4. 🎉

### What's Next?

Use `pet` in amazing ways:

List the snippets:

```
$ pet list
```

Search the snippets:

```
$ pet search
```

Add search result to the clipboard:

```
$ pet search | pbcopy
```

Interactively add your own snippet:

```
$ pet new
Command> curl -s <consul_http_addr>/v1/status/peers
Description> Get Consul server peers from HTTP API
```

See the [pet README](https://github.com/knqyf263/pet/blob/master/README.md) for more ways to use it with the snippets!

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

hashipets was created by [Brian Shumate](https://github.com/brianshumate) and made possible through the generous time of the good people named in [CONTRIBUTORS.md](https://github.com/brianshumate/hashipets/blob/master/CONTRIBUTORS.md)

## Special Thanks

Thanks to Teppei Fukuda for making pet!
