
<!--- This file is automatically generated by make gen-cli-docs; changes should be made in the go CLI command code (under cmd/kops) -->

## kops edit cluster

Edit cluster.

### Synopsis

Edit a cluster configuration.

This command changes the desired cluster configuration in the registry.

   To set your preferred editor, you can define the EDITOR environment variable.
   When you have done this, kOps will use the editor that you have set.

kops edit does not update the cloud resources; to apply the changes use `kops update cluster`.

```
kops edit cluster [flags]
```

### Examples

```
  # Edit a cluster configuration in AWS.
  kops edit cluster k8s.cluster.site --state=s3://my-state-store
```

### Options

```
  -h, --help            help for cluster
      --set strings     Directly set values in the spec
      --unset strings   Directly unset values in the spec
```

### Options inherited from parent commands

```
      --config string   yaml config file (default is $HOME/.kops.yaml)
      --name string     Name of cluster. Overrides KOPS_CLUSTER_NAME environment variable
      --state string    Location of state storage (kops 'config' file). Overrides KOPS_STATE_STORE environment variable
  -v, --v Level         number for the log level verbosity
```

### SEE ALSO

* [kops edit](kops_edit.md)	 - Edit clusters and other resources.

