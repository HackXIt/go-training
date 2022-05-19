# go-training
Personal library for learning the Go programming language and educating myself with the help of available online resources

## Note about Antivirus

For some reason, my antivirus software thinks that my compiled binary is a threat when using `go run`.
To work around this issue, I'm required to set GOTMPDIR to an appropriate folder and exclude said folder in the antivirus software, so I can safely run `go run`.
This only affects `go run`, calling `go build` and then executing the binary works fine.
It's also not the antivirus software fault, because when using `go run`, the binaries are compiled into the OS 'tmp' folder and then another program is called for executing said binary, which triggers red flags for the antivirus.

I'm not an expert on the details, but it is kind of an annoying issue to have, when starting to learn a language.