# FCC EA Exhibits

## COVID-19 Policy

- Stay inside, find 0-days

- Don't take medical advice from anyone who stares directly into the sun

## Status - 03/25/2020

- 1M exhibits are live (16.2K grantees)

- 2.1M more exhibits (30.4K grantees) are on the way

- second batch of exhibits will go live on the ~30th

## Wat is this?

Since all my hardware and radio hacker friends are stuck inside, I thought it might be fun to provide a distraction. To that end, I decided to push an annotated FCC EA exhibit dataset to a series of public git repos.

Each repository represents 1 grantee (company).

Exhibits in the repositories are structured as follows:

```
./fcc-id/application-id/exhibit-id.ext
```

Each repository contains the FCC-published exhibit documents that the grantee submitted to the FCC as part of the device certification process.

These exhibits can include **internal photos**, **external photos**, **RF test reports**, **block diagrams**, **operational descriptions**, **schematics**, **user manuals**, and various **correspondence**.

The top-level directories are sliced by the FCC ID of each device.

The second-level directories are named according to the application UUIDs. *Each FCC ID includes one or more application.*

Within each application directory are the exhibits submitted with that application. 

## Exhibit Manifest

Each repository contains a JSON manifest which provides metadata about each exhibit.

```
./manifest.json
```

JSON manifest includes the following metadata about each exhibit published by the FCC.

- FCC ID
- Grantee Code
- Product Code
- MD5
- Path
- File Extension
- Content Type
- Size
- Exhibit ID
- Exhibit Description
- Exhibit Type
- Date Submitted
- Date Available
- Grant Notes

## Grantee Manifest - 03/25/2020

16.2K grantees are currently live, with another 30.4K on the way.

This repository includes a compressed JSON manifest covering all exhibits and grantees currently live.

```
./master-manifest.json.zip
```

