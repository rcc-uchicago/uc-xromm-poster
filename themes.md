## Themes

* data pipelines
* data management
* streamlining research workflows
* research datasets (packaging/publishing)
* reproducible research

High-level sketch of the semi-automated XROMM dataset production pipeline:

    ROSS LAB                        RCC MIDWAY                XMA PORTAL
    E X P E R I M E N T S                                  D A T A S E T
    data acquisition > processing > replication 
                                        storage > packaging > publishing 
                                        |
                                        + file/blob storage (trial datafiles)
                                        + db-storage (trial metadata)

---

The XMA Portal provides an access and discovery platform for experimental data (calibration files, raw video data, 3D models) and metadata (trial date, experimenter, provenance, access restrictions, etc.).

However accessing XROMM data for analysis remains a bottleneck in the workflow. The XMA Portal could potentially take over data processing tasks (on a local server), delivering a package of video data, metadata, and calibration images to the analysis platform, and then receiving processed data and information about the analysis process (i.e. provenance) and cataloging them back into the database.
