# cowsay presentation systems

An optimized presentation software, written on the commuter rail train on the way to Grand Central Station.

As presented during my Wordhack September 2024 presentation at Wonderville, in Brooklyn, NY.

=> [Video on Youtube](https://youtu.be/jBCQ8EPpbgQ)  

This system uses the classic Linux cowsay software to make a presentation, voiced as well using espeak text to speech. The individual projects need to be launched however you like, from the command line, via a web browser, etc.

## Screenshot and Asciinema recording

[![asciicast](https://asciinema.org/a/PNyENmjcQx6UtKH4r4uiMNTfg.svg)](https://asciinema.org/a/PNyENmjcQx6UtKH4r4uiMNTfg)

## Requirements

* fish shell
* cowsay
* espeak

Note: Check to make sure your cowsay file has the same options as mine. `cowsay -l`. Some cowsay files may be inappropriate or NSFW. You may need to make adjustments.

## Install

```
git clone https://github.com/lee2sman/cowsay-presentation-systems.git
```

Inside sources directior edit:  
* intro.txt 
* bio.txt
* why.txt
* contact.txt
* works.txt

The works.txt file should match the projects you will be showing. One line per work. No blank lines.

## Run your presentation

You will probably want to `chmod +x *` (the presentation programs) in order to have permission to execute all of the files, or else you'll have to individually run `fish filename` to launch each of them.

### Introduce yourself

```sh
./introduction
```

### List all of your works

```sh
./everything
```

### Select the next project randomly

```sh
./next
```

### When you've made a mistake

```sh
./oops
```

### When you don't want to show one of the selections

```sh
./no
```

### Finish

```sh
./thanks
```
