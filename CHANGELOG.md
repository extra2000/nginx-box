# Changelog

### [2.0.1](https://github.com/extra2000/nginx-box/compare/v2.0.0...v2.0.1) (2021-05-16)


### Fixes

* **nginx-formula:** patch update to `v3.0.1` ([9abc493](https://github.com/extra2000/nginx-box/commit/9abc4931c4b79ddcbaae55664cb9110c1dea2e74))

## [2.0.0](https://github.com/extra2000/nginx-box/compare/v1.2.0...v2.0.0) (2021-05-15)


### ⚠ BREAKING CHANGES

* **zabbix-agent-formula:** `zabbix-agent-formula` has breaking changes and `salt/roots/pillar/zabbix-agent.sls.example` has changed.
* **nginx-formula:** `nginx-formula` has breaking changes.
* **podman-formula:** Submodule `podman-formula` has breaking changes.

### Features

* **nginx-formula:** upgrade from `v2.0.0` to `v3.0.0` ([bbda30c](https://github.com/extra2000/nginx-box/commit/bbda30ccd02b3584d38ffb45922e86b81c31c383))
* **podman-formula:** add `salt/roots/pillar/podman.sls.example` ([13f0d29](https://github.com/extra2000/nginx-box/commit/13f0d29038a58e311007a0cd4a51a202b409cc92))
* **podman-formula:** upgrade from `v2.2.1` to `v4.0.0` ([b4a7e11](https://github.com/extra2000/nginx-box/commit/b4a7e11838429a3d8fea7a1426eab11365d03047))
* **vagrant:** add Fedora 34 Vagrant file ([294695a](https://github.com/extra2000/nginx-box/commit/294695aaa0fc64524b31802e03b12db1846a5ec7))
* **zabbix-agent-formula:** upgrade from `v2.0.1` to `v5.0.0` ([a3d4a9a](https://github.com/extra2000/nginx-box/commit/a3d4a9aa153a3444cfecce60b6c667cd4e24a09a))


### Code Refactoring

* **podman-formula:** remove `salt/roots/pillar/podman.sls` and add into `.gitignore` ([2c0ff1b](https://github.com/extra2000/nginx-box/commit/2c0ff1b133521a241b3e62f08cc716940a84684c))


### Documentations

* **README:** add instruction to create `salt/roots/pillar/podman.sls` ([3444638](https://github.com/extra2000/nginx-box/commit/34446385c6ffb30550dd5bfce32a92c81bfc9441))
* **README:** change Fedora 33 to Fedora 34 ([f07dec4](https://github.com/extra2000/nginx-box/commit/f07dec4e42d30d1cce99d874f80b80bd28d990fb))


### Continuous Integrations

* **AppVeyor:** add instruction to create `salt/roots/pillar/podman.sls` ([af8fec8](https://github.com/extra2000/nginx-box/commit/af8fec8b1daef57fea69d954a788c83e81366131))
* **AppVeyor:** change Fedora 33 to Fedora 34 ([6716015](https://github.com/extra2000/nginx-box/commit/6716015bf86445f9b0172799c77ce8b177bb7237))
* **AppVeyor:** remove NGINX formula error workaround ([b5086e9](https://github.com/extra2000/nginx-box/commit/b5086e943c242f7eed1fee11b5f7675372c0e510))

## [1.2.0](https://github.com/extra2000/nginx-box/compare/v1.1.0...v1.2.0) (2021-03-15)


### Features

* **submodule:** Upgrade `filebeat-formula` to [v2.1.0](https://github.com/extra2000/filebeat-formula/releases/tag/v2.1.0) ([180a4d4](https://github.com/extra2000/nginx-box/commit/180a4d4ece427981601263e75e841a29c248637d))


### Documentations

* **README:** Add instruction to deploy Filebeat ([8d9ad79](https://github.com/extra2000/nginx-box/commit/8d9ad799115f229073401c874ce3edee633fcc73))

## [1.1.0](https://github.com/extra2000/nginx-box/compare/v1.0.0...v1.1.0) (2021-03-14)


### Features

* **submodule:** Add [filebeat-formula v2.0.0](https://github.com/extra2000/filebeat-formula/releases/tag/v2.0.0) ([b93eb6f](https://github.com/extra2000/nginx-box/commit/b93eb6f5491690b96984fb6b4cb7c503f9748e24))
* **submodule:** Add [podman-formula v2.2.1](https://github.com/extra2000/podman-formula/releases/tag/v2.2.1) ([c382cb8](https://github.com/extra2000/nginx-box/commit/c382cb8974da06400ff88b63f3ba9bab623e7aff))
* **submodule:** Add [zabbix-agent-formula v2.0.1](https://github.com/extra2000/zabbix-agent-formula/releases/tag/v2.0.1) ([7026a3d](https://github.com/extra2000/nginx-box/commit/7026a3d709b141c6245d509c7c65cf69a547b0e7))
* **submodule:** Update `nginx-formula` to [v2.0.0](https://github.com/extra2000/nginx-formula/releases/tag/v2.0.0) ([c83600d](https://github.com/extra2000/nginx-box/commit/c83600d096fa557f5fed2f4f2d07159ac188a212))


### Fixes

* **/etc/minion:** Using new style for `module.run` ([81a0a05](https://github.com/extra2000/nginx-box/commit/81a0a05116c85afb30d310a70cbc87e9c4ce02b0))


### Continuous Integrations

* **AppVeyor:** Update instructions prior to `nginx-formula` version [v2.0.0](https://github.com/extra2000/nginx-formula/releases/tag/v2.0.0) ([4d4de40](https://github.com/extra2000/nginx-box/commit/4d4de406b4cab3aef0b911c40cef0bc7fea94bb5))


### Documentations

* **README:** Update `README.md` ([e5aff59](https://github.com/extra2000/nginx-box/commit/e5aff59db0f9923df768a8966c3be497ed327d9c))

## 1.0.0 (2021-03-01)


### Features

* **salt:** Add implementations for states in `salt/` ([4796c9f](https://github.com/extra2000/nginx-box/commit/4796c9f3d5ee64e55b9f7df2d6777272f0cacf84))
* **submodule:** Add [nginx-formula v1.0.0](https://github.com/extra2000/nginx-formula/releases/tag/v1.0.0) ([62af883](https://github.com/extra2000/nginx-box/commit/62af883ffd2a175162cf3a4d35e9dc77fec2035f))
* **vagrant:** Import Vagrant files from [extra2000/generic-box v1.5.0](https://github.com/extra2000/generic-box/releases/tag/v1.5.0) ([4bf6066](https://github.com/extra2000/nginx-box/commit/4bf606655bfeba1f15620f171f45b6f81158a01e))


### Continuous Integrations

* Add AppVeyor with `semantic-release` bot ([d068e41](https://github.com/extra2000/nginx-box/commit/d068e412941ec9784e1e65173275dc5086969e3f))


### Documentations

* **README:** Update `README.md` ([30431c3](https://github.com/extra2000/nginx-box/commit/30431c395aa0b47c2533d357cfa498b7ccef9740))
