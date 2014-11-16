# UT64-fend

[protean/C764-fend](https://vagrantcloud.com/protean/boxes/C764-fend) is a standard CentOS 7 BASE box with LAMP(WP-CLI ready), NodeJS(via nodebrew), MongoDB, Redis, Ruby(via rbenv), Git and some helpful programs for front-end developers.

[EPEL](https://fedoraproject.org/wiki/EPEL)/[IUS](https://iuscommunity.org/pages/About.html)/[Remi](http://rpms.famillecollet.com/) repositories ready.

---

## Changelog

Initial release.

## Changelog(Box)

* Ver. 1.0.0: Initial release.

---

## Usage

1. Clone this repository
2. Vagrant up
3. Vagrant ssh
4. Run `sudo yum update`
5. Open [http://192.168.33.200](http://192.168.33.200).

## Update softwares

### RPM

```
$ sudo yum update
```

### npm

Nodejs installed via [nodebrew](https://github.com/hokaccha/nodebrew). Check update with david.

```
$ david -g
$ npm install -g (updated-packages)
```

### gem

Ruby installed via rbenv. rbenv-rehash is already installed.

```
$ gem update
```

### composer

```
$ composer selfupdate
```

### WP-CLI (via Composer)

```
$ cd ~/.composer
$ composer update
```

## Box info.

* Box root passwd: vagrant
* MySQL login: root/root
* PHP info: [http://192.168.33.200/info.php](http://192.168.33.200/info.php)

Connect to MySQL and MongoDB w/ SSH（Host: 192.168.33.200, id: vagrant, password: vagrant）.
