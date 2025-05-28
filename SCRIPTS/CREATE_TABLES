/*==========================================
DDL SCRIPT: create BRONZE TABLES
=============================================
THIS SCRIPT CREATES BRONZE_LAYER TABLES,DROPPING TABLES IF THEY EXIST ALREADY.
RUN THIS SCRIPT TO RE-DEFINE THE DDL STRUCTURE OF 'BRONZE' TABLES.*/


IF OBJECT_ID('bronze.crm_cust_info','U') IS NOT NULL
	DROP TABLE bronze.crm_cust_info;
GO
CREATE TABLE bronze.crm_cust_info(
	cst_id INT,
	CST_KEY NVARCHAR(50),
	CST_FIRSTNAME NVARCHAR(50),
	CST_LASTNAME NVARCHAR(50),
	CST_MARITAL_STATUS NVARCHAR(50),
	CST_GNDR NVARCHAR(50),
	CST_CREATE_DATE DATE
);

IF OBJECT_ID('BRONZE.CRM_PRD_INFO','U') IS NOT NULL
	DROP TABLE BRONZE.CRM_PRD_INFO;
GO
CREATE TABLE BRONZE.CRM_PRD_INFO(
	prd_id INT,
	prd_key NVARCHAR(50),
	prd_nm NVARCHAR(50),
	prd_cost INT,
	prd_line NVARCHAR(50),
	prd_start_dt DATE,
	prd_end_dt DATE
)

IF OBJECT_ID('BRONZE.CRM_SALES_DETAILS','U') IS NOT NULL
	DROP TABLE BRONZE.CRM_SALES_DETAILS;
GO
CREATE TABLE BRONZE.CRM_SALES_DETAILS(
	sls_ord_num NVARCHAR(50),
	sls_prd_key NVARCHAR(50),
	sls_cust_id INT,
	sls_order_dt INT,
	sls_ship_dt INT,
	sls_due_dt INT,
	sls_sales INT,
	sls_quantity INT,
	sls_price INT
	)
GO

IF OBJECT_ID('bronze.erp_cust_az12','U') is not NULL
	DROP TABLE bronze.erp_cust_az12;
GO
CREATE TABLE bronze.erp_cust_az12(
	cid NVARCHAR(50),
	bdate NVARCHAR(50),
	gen NVARCHAR(50)
)

IF OBJECT_ID('bronze.erp_loc_a101','U') is not NULL
	DROP TABLE bronze.erp_loc_a101;
GO
CREATE TABLE bronze.erp_loc_a101(
	cid NVARCHAR(50),
	cntry NVARCHAR(50)
)

IF OBJECT_ID('bronze.erp_px_cat_g1v2','U') is not NULL
	DROP TABLE bronze.erp_px_cat_g1v2;
GO
CREATE TABLE bronze.erp_px_cat_g1v2(
	id NVARCHAR(50),
	cat NVARCHAR(50),
	subcat NVARCHAR(50),
	maintenance NVARCHAR(50)
)
	


