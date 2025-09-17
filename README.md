# VM Lifecycle on GCP and OCI — Tutorial

## Video
Loom for Oracle: <[Oracle](https://www.loom.com/share/672718a4976848e489915177dad642a4?sid=a22cc99b-40eb-4029-ac9e-bcbcb0c0c702)>

Loom for Google Cloud: <[Google Cloud](https://www.loom.com/share/a8c8fb52462748e8b4a154b66217c46d?sid=ed58b8b3-cd6f-412e-88e7-f4a7914db586)>

## Prereqs
- Cloud access to GCP and OCI
- No PHI/PII; smallest/free-tier shapes

---

## Google Cloud (GCP)
### Create
1. Console → Compute Engine → Create instance
2. Region/zone: <East(Northern Virgina)>
3. Machine type: <e2-micro>
4. Image: Ubuntu LTS
5. Boot disk: default minimal
6. Network: default VPC; ephemeral public IP

![GCP create](images/GCI_create.png)

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