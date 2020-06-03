Run the Apache Jena riot tool to validate or convert RDF to RDF.

Use Docker Image from https://hub.docker.com/r/stain/jena

## Usage

### Validate RDF

```yaml
- uses: vemonet/rdfhdt-action@master
  with:
    input: my_file.nt
    output: my_file.hdt
```

### Convert RDF to RDF

```yaml
- uses: vemonet/jena-riot-action@master
  with:
  	operation: hdt2rdf
    input: my_file.hdt
    output: my_file.nt
```

