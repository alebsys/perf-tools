# Perf tools

## Adding `bpftrace` Utilities to Your PATH

So you can run your `.bt` scripts from anywhere:

### Temporary (current session)

```bash
git clone https://github.com/alebsys/perf-tools.git
cd perf-tools
export PATH="$(pwd)/bpftrace:$PATH"
```

### Permanent (every new shell)
```bash
git clone https://github.com/alebsys/perf-tools.git
cd perf-tools
echo 'export PATH="$(pwd)/bpftrace:$PATH"' >> ~/.bashrc && source ~/.bashrc
```
