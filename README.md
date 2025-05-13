# Perf tools

## Adding `bpftrace` Utilities to Your PATH

So you can run your `.bt` scripts from anywhere:

### Temporary (current session)

```bash
git clone https://github.com/alebsys/perf-tools.git
cd perf-tools
chmod +x bpftrace/*
export PATH="$(pwd)/bpftrace:$PATH"
```

### Permanent (every new shell)
```bash
git clone https://github.com/alebsys/perf-tools.git
cd perf-tools
chmod +x bpftrace/*
echo 'export PATH="$(pwd)/bpftrace:$PATH"' >> ~/.bashrc && source ~/.bashrc
```
