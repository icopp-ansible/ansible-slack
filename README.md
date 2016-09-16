# ansible-slack

Install Slack via the Mac App Store or Homebrew Cask.

## Role Variables

* `prefer_mas_over_homebrew`: Defaults to `false`.

## Dependencies

* [icopp.mas-cli](https://github.com/icopp/ansible-mas-cli), but only if `prefer_mas_over_homebrew` is `true`.
* [icopp.homebrew-cask](https://github.com/icopp/ansible-homebrew-cask), but only if `prefer_mas_over_homebrew` is `false`.

## Example Playbook

```
  - hosts: all
    roles:
      - role: icopp.slack
```

```
  - hosts: all
    roles:
      - role: icopp.slack
        prefer_mas_over_homebrew: true
```

## License

MIT
