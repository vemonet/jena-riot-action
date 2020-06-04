Run the Apache Jena riot tool to validate or convert RDF to RDF.

Use Docker Image from https://hub.docker.com/r/stain/jena

## Usage

### Validate RDF

```yaml
- uses: vemonet/jena-riot-action@v3.14
  with:
    input: my_file.ttl
```

### Convert RDF to RDF

```yaml
- uses: vemonet/jena-riot-action@v3.14
  with:
    input: my_file.ttl
    convert: --output=NQUADS
```

> Jena does not allow to output to file directly. Would need to rewrite entrypoint.