# DAIS 2025 GenAI Hackathon

## 1. Set Up Your Workspace and Get Data

### Setting up your Workspace

Use the provided link to get your Databricks trial account. This will be provided on the day of the hackathon.

### Getting the Data

Our *Data for Good* partners are providing several datasets for you to use in this hackathon. To access the data, you will need to configure your Databricks workspace to use Delta Sharing and then provide your Delta Sharing ID to the hackathon organizers.

#### Granting `USE PROVIDER` Privileges

To receive data via Delta Sharing, you will need `USE PROVIDER` privileges on your Unity Catalog metastore. To grant this, you can use the following approach:

1. Navigate to the "Catalog" tab in the left sidebar of your Databricks workspace.

![Navigate to Catalog](./images/1_catalog.png)

2.  Click the gear symbol ("Manage") and select "Metastore" from the dropdown menu.

![Navigate to Metastore](./images/2_metastore.png)

3.  Click the "Permissions" tab and then click the "Grant" button.

![Grant Permissions](./images/3_grant.png)

4. Check the box next to `USE PROVIDER` and select "All Account Users" from the "Principals" dropdown menu.

![Use Provider](./images/4_use_provider.png)

5. Click "Grant" to set the privilege.

For more information, see the [Delta Sharing documentation on reading shared data](https://docs.databricks.com/aws/en/delta-sharing/read-data-databricks#permissions-required).

#### Obtain and Share your Delta Sharing ID

Once you have been granted `USE PROVIDER` privileges, you can obtain your Delta Sharing ID by clicking the "Copy" button in the "Delta Sharing" section of the "Settings" tab. You will then provide this ID to the hackathon organizers via a google form that will be provided on the day of the hackathon.

1. Navigate to the "Catalog" tab in the left sidebar of your Databricks workspace and then click the "Delta Sharing" button.

![Navigate to Delta Sharing](./images/5_delta_sharing.png)

2. Click your Databricks sharing organization name in the upper right, and select Copy sharing identifier.

![Copy Sharing Identifier](./images/6_copy_sharing_id.png)

3. Share your Delta Sharing ID with the hackathon organizers using the provided Google form.

After we have received your Delta Sharing ID, we will share the data to your Databricks account. From the Catalog -> Delta Sharing menu, in the "Shared with me" tab, you will see the share. To use the data, click on the share name, and then click "Create catalog" next to the dataset you would like to use. This will create a new catalog in your Databricks workspace with the shared data, and you can start using it immediately.

![Create Catalog](./images/7_create_catalog.png)