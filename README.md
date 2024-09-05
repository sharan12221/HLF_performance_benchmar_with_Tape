# HLF_performance_benchmar_with_Tape

A light-weight tool to test performance of Hyperledger Fabric  It is used to perform super simple performance test. Our main focus is to make sure that tape will not be the bottleneck of performance test

# steps

1) Install tape binarys
```
chmod +x install.sh
./install.sh
```

2) run commitOnly 
```
./tape-Linux-X64 commitOnly --config=config.yaml --number=2000
```

3) run endorsementOnly 
```
./tape-Linux-X64 endorsementOnly --config=config.yaml --number=2000
```

4) run complete transaction
```
./tape-Linux-X64 --config=config.yaml --number=2000
```