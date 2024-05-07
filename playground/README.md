# K8S namespaced playground

It build a safe, namespace-isolated environment so that Kubernetes can be used for experiential purposes such as general user or developer training.

## Dependencies

- jinja2 `pip install jinja2`
- justfile `sudo apt-get install just`
- kubectl
- runs on control plane

## Usage

### Create

```bash
# Define the team count
my_team_count=42

# Execute it!
just create $my_team_count

# The accounts would be generated in the `confs` directory
ls confs/
```

### Apply

```bash
# Define the team count
my_team_count=42

# Execute it!
just apply $my_team_count

# The accounts would be generated in the `confs` directory
ls confs/
```

### Delete

```bash
# Define the team count
my_team_count=42

# Execute it!
just delete $my_team_count
```

### Delete ALL teams

```bash
# Execute it!
just delete-all
```
