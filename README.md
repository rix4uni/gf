## gf

This is tomnomnom's tool [gf](https://github.com/tomnomnom/gf) so all credit goes to him, I just modified the code according to my requirements.

## Installation
```
go install github.com/rix4uni/gf@latest
```

## Download prebuilt binaries
```
wget https://github.com/rix4uni/gf/releases/download/v0.0.1/gf-linux-amd64-0.0.1.tgz
tar -xvzf gf-linux-amd64-0.0.1.tgz
rm -rf gf-linux-amd64-0.0.1.tgz
mv gf ~/go/bin/gf
```
Or download [binary release](https://github.com/rix4uni/gf/releases) for your platform.

## Compile from source
```
git clone --depth 1 github.com/rix4uni/gf.git
cd gf; go install
```

## Setup `gf-patterns` 
```
git clone https://github.com/rix4uni/gf-patterns.git ~/.garudrecon/.gf
```

## Usage
```
Usage of gf:
  -custom-path string
        specify a custom pattern file path
  -dump
        prints the grep command rather than executing it
  -list
        list available patterns
  -save
        save a pattern (e.g: gf -save pat-name -Hnri 'search-pattern')
```

## Examples Usages
```
▶ cat urls.txt | gf xss

OR

▶ cat urls.txt | gf -custom-path ~/.garudrecon/.gf xss
```