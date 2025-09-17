# VM Lifecycle on GCP and OCI — Tutorial

## Video
[GCP Tutorial] (https://www.loom.com/share/c1953f1fae2d4a7d99a4deb05a81e646?sid=cc470858-0c6f-46c0-b239-06b1aa59cd0f)
[OCI Tutorial & Reflection/Comparison of Both] (https://www.loom.com/share/3c24d4135e6c402f84176ed27194cdb5?sid=62756d51-d058-4078-8035-3edd5f2a2ebc)

## Prereqs
- Cloud access to GCP and OCI
- No PHI/PII; smallest/free-tier shapes

---

## Google Cloud (GCP)
### Create
1. Console → Compute Engine → Create instance
2. Region/zone: <your choice>
3. Machine type: <smallest available/free-eligible>
4. Image: Ubuntu LTS
5. Boot disk: default minimal
6. Network: default VPC; ephemeral public IP

![GCP create](images/gcp_create.png)

### Start/Stop
- Start: <state shows RUNNING>
- Stop: <state shows TERMINATED/STOPPED>

![GCP running](images/gcp_running.png)

### Delete
- Delete instance and verify no disks/IPs remain

![GCP cleaned](images/gcp_clean.png)

---

## Oracle Cloud (OCI)
### Create
1. Compartment: <name>
2. Networking: VCN with Internet Connectivity (defaults)
3. Shape: <smallest/free-eligible>
4. Image: Ubuntu (or Oracle Linux)
5. Public IP: ephemeral
6. Boot volume: default minimal

![OCI create](images/oci_create.png)

### Start/Stop
- Start: <state shows RUNNING>
- Stop: <state shows STOPPED>

![OCI running](images/oci_running.png)

### Terminate
- Terminate and delete boot volume; verify cleanup

![OCI cleaned](images/oci_clean.png)

---

## Reflections
### Similarities
- <brief bullets>

### Differences
- <brief bullets>

### Preference (OCI vs GCP) and Why
- <one short paragraph>