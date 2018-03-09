# ansible-elixir-centos7

This is a playbook for quickly installing the latest Erlang and Elixir releases onto a CentOS7 box.

All you need is a `hosts` file in the following format:

```
[elixir]
elixir-box-01 ansible_host=10.0.0.1
elixir-box-03 ansible_host=10.0.0.3

[removeelixir]
elixir-box-02 ansible_host=10.0.0.2
```

From here, you just run `ansible-playbook site.yml`.
