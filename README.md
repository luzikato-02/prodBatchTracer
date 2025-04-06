# Production Batch Tracer

## What is this for?
In my company, we have certain process issues that coming from our material deformities (properties or contaminations). Each upsteam process contains materials coming from multiple downsteam process batches which we need to trace. This tracing process is meant to identify any machine or process parameters abnormalities from downstream process which will be used as our main concern for improvement or repair.

## How it works?
Before we start our upstream process we will record every material batches that loaded into our material feeder machine through our ERP system. This record contains the batch number, material code, date of entry, and etc. However, this data can be developed to contain additional columns for analysis purposes if we need it. However, with so much information we get from our ERP system. It is still difficult for us to analyze and trace back each production batches since the materials are too many for human-brain to analyze. Hence, the development of this app.

This app will use two datatables:
1. The material feeder loading record
2. The material production report (downstream process)

All of which will taken from our ERP system database. However, this data cannot be streamlined directly to this app by any means since we are limited by our company policy. In this app, we will create somekind of datamodel that connects the loading data and production report in a way that we can summarize these main insights: machine number, date of production, and properties abnormalities.
