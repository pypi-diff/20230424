# Comparing `tmp/stigg_api_client-0.4.0.tar.gz` & `tmp/stigg_api_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.4.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.5.0.tar", max compression
```

## Comparing `stigg_api_client-0.4.0.tar` & `stigg_api_client-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-03-05 12:25:06.526402 stigg_api_client-0.4.0/README.md
--rw-r--r--   0        0        0      396 2023-04-23 10:58:44.895101 stigg_api_client-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-04-23 10:33:15.442973 stigg_api_client-0.4.0/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-04-23 10:31:23.415609 stigg_api_client-0.4.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-03-05 12:25:06.527730 stigg_api_client-0.4.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    43935 2023-04-12 14:11:36.612247 stigg_api_client-0.4.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   432273 2023-04-12 14:11:36.614988 stigg_api_client-0.4.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 stigg_api_client-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-03-05 12:25:06.526402 stigg_api_client-0.5.0/README.md
+-rw-r--r--   0        0        0      396 2023-04-24 14:47:14.271119 stigg_api_client-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-04-23 10:33:15.442973 stigg_api_client-0.5.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-04-24 07:23:15.920589 stigg_api_client-0.5.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-03-05 12:25:06.527730 stigg_api_client-0.5.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    44689 2023-04-24 14:46:41.477637 stigg_api_client-0.5.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   443944 2023-04-24 14:46:41.312733 stigg_api_client-0.5.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 stigg_api_client-0.5.0/PKG-INFO
```

### Comparing `stigg_api_client-0.4.0/README.md` & `stigg_api_client-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.4.0/stigg/client.py` & `stigg_api_client-0.5.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.4.0/stigg/generated/operations.py` & `stigg_api_client-0.5.0/stigg/generated/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -825,18 +825,24 @@
     _op_provision_customer_customer.__fragment__(fragment_slim_customer_fragment())
     _op_provision_customer.subscription_decision_strategy()
     _op_provision_customer_subscription = _op_provision_customer.subscription()
     _op_provision_customer_subscription.__fragment__(fragment_slim_subscription_fragment())
     return _op
 
 
+def mutation_import_customer_bulk():
+    _op = sgqlc.operation.Operation(_schema_root.mutation_type, name='ImportCustomerBulk', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.ImportCustomerBulk))))
+    _op.import_customers_bulk(input=sgqlc.types.Variable('input'))
+    return _op
+
+
 def mutation_import_customer():
     _op = sgqlc.operation.Operation(_schema_root.mutation_type, name='ImportCustomer', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.ImportCustomerInput))))
     _op_import_customer = _op.import_one_customer(input=sgqlc.types.Variable('input'), __alias__='import_customer')
-    _op_import_customer.__fragment__(fragment_customer_fragment())
+    _op_import_customer.__fragment__(fragment_slim_customer_fragment())
     return _op
 
 
 def mutation_update_customer():
     _op = sgqlc.operation.Operation(_schema_root.mutation_type, name='UpdateCustomer', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.UpdateCustomerInput))))
     _op_update_customer = _op.update_one_customer(input=sgqlc.types.Variable('input'), __alias__='update_customer')
     _op_update_customer.__fragment__(fragment_customer_fragment())
@@ -849,14 +855,20 @@
     _op_provision_subscription.checkout_url()
     _op_provision_subscription.status()
     _op_provision_subscription_subscription = _op_provision_subscription.subscription()
     _op_provision_subscription_subscription.__fragment__(fragment_slim_subscription_fragment())
     return _op
 
 
+def mutation_import_subscriptions_bulk():
+    _op = sgqlc.operation.Operation(_schema_root.mutation_type, name='ImportSubscriptionsBulk', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.ImportSubscriptionsBulk))))
+    _op.import_subscriptions_bulk(input=sgqlc.types.Variable('input'))
+    return _op
+
+
 def mutation_update_subscription():
     _op = sgqlc.operation.Operation(_schema_root.mutation_type, name='UpdateSubscription', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.UpdateSubscriptionInput))))
     _op_update_subscription = _op.update_one_subscription(input=sgqlc.types.Variable('input'), __alias__='update_subscription')
     _op_update_subscription.__fragment__(fragment_slim_subscription_fragment())
     return _op
 
 
@@ -921,14 +933,16 @@
 class Mutation:
     cancel_subscription = mutation_cancel_subscription()
     cancel_subscription_updates = mutation_cancel_subscription_updates()
     create_subscription = mutation_create_subscription()
     estimate_subscription = mutation_estimate_subscription()
     estimate_subscription_update = mutation_estimate_subscription_update()
     import_customer = mutation_import_customer()
+    import_customer_bulk = mutation_import_customer_bulk()
+    import_subscriptions_bulk = mutation_import_subscriptions_bulk()
     initiate_checkout = mutation_initiate_checkout()
     provision_customer = mutation_provision_customer()
     provision_subscription = mutation_provision_subscription()
     report_entitlement_check_requested = mutation_report_entitlement_check_requested()
     report_usage = mutation_report_usage()
     update_customer = mutation_update_customer()
     update_subscription = mutation_update_subscription()
```

### Comparing `stigg_api_client-0.4.0/stigg/generated/schema.py` & `stigg_api_client-0.5.0/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,19 @@
 
 
 class Currency(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('AED', 'ALL', 'AMD', 'ANG', 'AUD', 'AWG', 'AZN', 'BAM', 'BBD', 'BDT', 'BGN', 'BIF', 'BMD', 'BND', 'BSD', 'BWP', 'BYN', 'BZD', 'CAD', 'CDF', 'CHF', 'CLP', 'CNY', 'CZK', 'DJF', 'DKK', 'DOP', 'DZD', 'EGP', 'ETB', 'EUR', 'FJD', 'GBP', 'GEL', 'GIP', 'GMD', 'GNF', 'GYD', 'HKD', 'HRK', 'HTG', 'IDR', 'ILS', 'INR', 'ISK', 'JMD', 'JPY', 'KES', 'KGS', 'KHR', 'KMF', 'KRW', 'KYD', 'KZT', 'LBP', 'LKR', 'LRD', 'LSL', 'MAD', 'MDL', 'MGA', 'MKD', 'MMK', 'MNT', 'MOP', 'MRO', 'MVR', 'MWK', 'MXN', 'MYR', 'MZN', 'NAD', 'NGN', 'NOK', 'NPR', 'NZD', 'PGK', 'PHP', 'PKR', 'PLN', 'PYG', 'QAR', 'RON', 'RSD', 'RUB', 'RWF', 'SAR', 'SBD', 'SCR', 'SEK', 'SGD', 'SLE', 'SLL', 'SOS', 'SZL', 'THB', 'TJS', 'TOP', 'TRY', 'TTD', 'TZS', 'UAH', 'UGX', 'USD', 'UZS', 'VND', 'VUV', 'WST', 'XAF', 'XCD', 'XOF', 'XPF', 'YER', 'ZAR', 'ZMW')
 
 
+class CustomerResourceSortFields(sgqlc.types.Enum):
+    __schema__ = schema
+    __choices__ = ('createdAt', 'environmentId', 'resourceId')
+
+
 class CustomerSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('billingId', 'createdAt', 'crmHubspotCompanyId', 'crmHubspotCompanyUrl', 'crmId', 'customerId', 'email', 'environmentId', 'id', 'name', 'refId', 'updatedAt')
 
 
 class CustomerSubscriptionSortFields(sgqlc.types.Enum):
     __schema__ = schema
@@ -136,20 +141,20 @@
 class EnvironmentSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('createdAt', 'displayName', 'id', 'slug')
 
 
 class ErrorCode(sgqlc.types.Enum):
     __schema__ = schema
-    __choices__ = ('AccountNotFoundError', 'AddonHasToHavePriceError', 'AddonNotFound', 'ArchivedCouponCantBeApplied', 'AuthCustomerMismatch', 'BadUserInput', 'BillingPeriodMissingError', 'CannotDeleteCustomerError', 'CannotDeleteFeatureError', 'CannotEditPackageInNonDraftMode', 'CheckoutIsNotSupported', 'CheckoutOptionsMissing', 'CouponNotFound', 'CustomerAlreadyHaveCustomerCoupon', 'CustomerAlreadyUsesCoupon', 'CustomerHasNoPaymentMethod', 'CustomerNoBillingId', 'CustomerNotFound', 'CustomerResourceNotFound', 'DowngradeBillingPeriodNotSupportedError', 'DraftPlanCantBeArchived', 'DuplicatedEntityNotAllowed', 'EditAllowedOnDraftPackageOnlyError', 'EntitlementsMustBelongToSamePackage', 'EntityIdDifferentFromRefIdError', 'EnvironmentMissing', 'ExperimentAlreadyRunning', 'ExperimentNotFoundError', 'ExperimentStatusError', 'FailedToCreateCheckoutSessionError', 'FailedToImportCustomer', 'FeatureNotFound', 'FetchAllCountriesPricesNotAllowed', 'IdentityForbidden', 'ImportAlreadyInProgress', 'InitStripePaymentMethodError', 'IntegrationNotFound', 'IntegrityViolation', 'InvalidAddressError', 'InvalidArgumentError', 'InvalidCancellationDate', 'InvalidEntitlementResetPeriod', 'InvalidMemberDelete', 'InvalidQuantity', 'InvalidSubscriptionStatus', 'InvalidUpdatePriceUnitAmountError', 'InvalidUsageValueForIncrementalFeatureError', 'MemberInvitationError', 'MemberNotFound', 'MeteringNotAvailableForFeatureType', 'MissingEntityIdError', 'NoFeatureEntitlementInSubscription', 'NoProductsAvailable', 'OperationNotAllowedDuringInProgressExperiment', 'PackageAlreadyPublished', 'PackagePricingTypeNotSet', 'PlanAlreadyExtended', 'PlanCannotBePublishWhenBasePlanIsDraft', 'PlanIsUsedAsDefaultStartPlan', 'PlanIsUsedAsDowngradePlan', 'PlanNotFound', 'PlanWithChildCantBeDeleted', 'PlansCircularDependencyError', 'PriceNotFound', 'PromotionCodeCustomerNotFirstPurchase', 'PromotionCodeMaxRedemptionsReached', 'PromotionCodeMinimumAmountNotReached', 'PromotionCodeNotActive', 'PromotionCodeNotForCustomer', 'PromotionCodeNotFound', 'RateLimitExceeded', 'ResyncAlreadyInProgress', 'SelectedBillingModelDoesntMatchImportedItemError', 'StripeCustomerIsDeleted', 'SubscriptionAlreadyCanceledOrExpired', 'SubscriptionMustHaveSinglePlanError', 'SubscriptionNotFound', 'TrialMinDateError', 'TrialMustBeCancelledImmediately', 'UnPublishedPackage', 'Unauthenticated', 'UncompatibleSubscriptionAddon', 'UnexpectedError', 'UnsupportedFeatureType', 'UnsupportedSubscriptionScheduleType', 'UnsupportedVendorIdentifier')
+    __choices__ = ('AccountNotFoundError', 'AddonHasToHavePriceError', 'AddonNotFound', 'ArchivedCouponCantBeApplied', 'AuthCustomerMismatch', 'BadUserInput', 'BillingPeriodMissingError', 'CannotDeleteCustomerError', 'CannotDeleteFeatureError', 'CannotDeleteProductError', 'CannotEditPackageInNonDraftMode', 'CheckoutIsNotSupported', 'CheckoutOptionsMissing', 'CouponNotFound', 'CustomerAlreadyHaveCustomerCoupon', 'CustomerAlreadyUsesCoupon', 'CustomerHasNoPaymentMethod', 'CustomerNoBillingId', 'CustomerNotFound', 'CustomerResourceNotFound', 'DowngradeBillingPeriodNotSupportedError', 'DraftPlanCantBeArchived', 'DuplicatedEntityNotAllowed', 'EditAllowedOnDraftPackageOnlyError', 'EntitlementsMustBelongToSamePackage', 'EntityIdDifferentFromRefIdError', 'EnvironmentMissing', 'ExperimentAlreadyRunning', 'ExperimentNotFoundError', 'ExperimentStatusError', 'FailedToCreateCheckoutSessionError', 'FailedToImportCustomer', 'FeatureNotFound', 'FetchAllCountriesPricesNotAllowed', 'IdentityForbidden', 'ImportAlreadyInProgress', 'InitStripePaymentMethodError', 'IntegrationNotFound', 'IntegrityViolation', 'InvalidAddressError', 'InvalidArgumentError', 'InvalidCancellationDate', 'InvalidEntitlementResetPeriod', 'InvalidMemberDelete', 'InvalidQuantity', 'InvalidSubscriptionStatus', 'InvalidUpdatePriceUnitAmountError', 'InvalidUsageValueForIncrementalFeatureError', 'MemberInvitationError', 'MemberNotFound', 'MeteringNotAvailableForFeatureType', 'MissingEntityIdError', 'NoFeatureEntitlementInSubscription', 'NoProductsAvailable', 'OperationNotAllowedDuringInProgressExperiment', 'PackageAlreadyPublished', 'PackagePricingTypeNotSet', 'PlanAlreadyExtended', 'PlanCannotBePublishWhenBasePlanIsDraft', 'PlanIsUsedAsDefaultStartPlan', 'PlanIsUsedAsDowngradePlan', 'PlanNotFound', 'PlanWithChildCantBeDeleted', 'PlansCircularDependencyError', 'PriceNotFound', 'PromotionCodeCustomerNotFirstPurchase', 'PromotionCodeMaxRedemptionsReached', 'PromotionCodeMinimumAmountNotReached', 'PromotionCodeNotActive', 'PromotionCodeNotForCustomer', 'PromotionCodeNotFound', 'RateLimitExceeded', 'ResyncAlreadyInProgress', 'SelectedBillingModelDoesntMatchImportedItemError', 'StripeCustomerIsDeleted', 'SubscriptionAlreadyCanceledOrExpired', 'SubscriptionMustHaveSinglePlanError', 'SubscriptionNotFound', 'TrialMinDateError', 'TrialMustBeCancelledImmediately', 'UnPublishedPackage', 'Unauthenticated', 'UncompatibleSubscriptionAddon', 'UnexpectedError', 'UnsupportedFeatureType', 'UnsupportedSubscriptionScheduleType', 'UnsupportedVendorIdentifier')
 
 
 class EventLogType(sgqlc.types.Enum):
     __schema__ = schema
-    __choices__ = ('ADDON_CREATED', 'ADDON_DELETED', 'ADDON_UPDATED', 'COUPON_ARCHIVED', 'COUPON_CREATED', 'COUPON_UPDATED', 'CREATE_SUBSCRIPTION_FAILED', 'CUSTOMER_CREATED', 'CUSTOMER_DELETED', 'CUSTOMER_PAYMENT_FAILED', 'CUSTOMER_RESOURCE_ENTITLEMENT_CALCULATION_TRIGGERED', 'CUSTOMER_UPDATED', 'EDGE_API_DATA_RESYNC', 'ENTITLEMENTS_UPDATED', 'ENTITLEMENT_DENIED', 'ENTITLEMENT_GRANTED', 'ENTITLEMENT_REQUESTED', 'ENVIRONMENT_DELETED', 'FEATURE_CREATED', 'FEATURE_DELETED', 'FEATURE_UPDATED', 'IMPORT_INTEGRATION_CATALOG_TRIGGERED', 'IMPORT_INTEGRATION_CUSTOMERS_TRIGGERED', 'MEASUREMENT_REPORTED', 'PACKAGE_PUBLISHED', 'PLAN_CREATED', 'PLAN_DELETED', 'PLAN_UPDATED', 'PRODUCT_CREATED', 'PRODUCT_DELETED', 'PRODUCT_UPDATED', 'PROMOTIONAL_ENTITLEMENT_EXPIRED', 'PROMOTIONAL_ENTITLEMENT_GRANTED', 'PROMOTIONAL_ENTITLEMENT_REVOKED', 'PROMOTIONAL_ENTITLEMENT_UPDATED', 'RESYNC_INTEGRATION_TRIGGERED', 'SUBSCRIPTION_CANCELED', 'SUBSCRIPTION_CREATED', 'SUBSCRIPTION_EXPIRED', 'SUBSCRIPTION_TRIAL_CONVERTED', 'SUBSCRIPTION_TRIAL_ENDS_SOON', 'SUBSCRIPTION_TRIAL_EXPIRED', 'SUBSCRIPTION_TRIAL_STARTED', 'SUBSCRIPTION_UPDATED', 'SUBSCRIPTION_USAGE_UPDATED', 'SYNC_FAILED', 'WIDGET_CONFIGURATION_UPDATED')
+    __choices__ = ('ADDON_CREATED', 'ADDON_DELETED', 'ADDON_UPDATED', 'COUPON_ARCHIVED', 'COUPON_CREATED', 'COUPON_UPDATED', 'CREATE_SUBSCRIPTION_FAILED', 'CUSTOMER_CREATED', 'CUSTOMER_DELETED', 'CUSTOMER_ENTITLEMENT_CALCULATION_TRIGGERED', 'CUSTOMER_PAYMENT_FAILED', 'CUSTOMER_RESOURCE_ENTITLEMENT_CALCULATION_TRIGGERED', 'CUSTOMER_UPDATED', 'EDGE_API_DATA_RESYNC', 'ENTITLEMENTS_UPDATED', 'ENTITLEMENT_DENIED', 'ENTITLEMENT_GRANTED', 'ENTITLEMENT_REQUESTED', 'ENVIRONMENT_DELETED', 'FEATURE_CREATED', 'FEATURE_DELETED', 'FEATURE_UPDATED', 'IMPORT_INTEGRATION_CATALOG_TRIGGERED', 'IMPORT_INTEGRATION_CUSTOMERS_TRIGGERED', 'MEASUREMENT_REPORTED', 'PACKAGE_PUBLISHED', 'PLAN_CREATED', 'PLAN_DELETED', 'PLAN_UPDATED', 'PRODUCT_CREATED', 'PRODUCT_DELETED', 'PRODUCT_UPDATED', 'PROMOTIONAL_ENTITLEMENT_EXPIRED', 'PROMOTIONAL_ENTITLEMENT_GRANTED', 'PROMOTIONAL_ENTITLEMENT_REVOKED', 'PROMOTIONAL_ENTITLEMENT_UPDATED', 'RESYNC_INTEGRATION_TRIGGERED', 'SUBSCRIPTION_CANCELED', 'SUBSCRIPTION_CREATED', 'SUBSCRIPTION_EXPIRED', 'SUBSCRIPTION_TRIAL_CONVERTED', 'SUBSCRIPTION_TRIAL_ENDS_SOON', 'SUBSCRIPTION_TRIAL_EXPIRED', 'SUBSCRIPTION_TRIAL_STARTED', 'SUBSCRIPTION_UPDATED', 'SUBSCRIPTION_USAGE_UPDATED', 'SYNC_FAILED', 'WIDGET_CONFIGURATION_UPDATED')
 
 
 class ExperimentSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('createdAt', 'environmentId', 'id', 'name', 'productId', 'refId', 'status')
 
 
@@ -396,14 +401,19 @@
 
 
 class UsageMeasurementSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('createdAt', 'environmentId', 'id')
 
 
+class UsageUpdateBehavior(sgqlc.types.Enum):
+    __schema__ = schema
+    __choices__ = ('DELTA', 'SET')
+
+
 class VendorIdentifier(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('HUBSPOT', 'STRIPE', 'ZUORA')
 
 
 class WeeklyAccordingTo(sgqlc.types.Enum):
     __schema__ = schema
@@ -915,14 +925,77 @@
 class CustomerPortalInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('customer_id', 'resource_id')
     customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
 
 
+class CustomerResourceFilter(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('and_', 'created_at', 'customer', 'environment_id', 'or_', 'resource_id', 'subscriptions')
+    and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilter')), graphql_name='and')
+    created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
+    customer = sgqlc.types.Field('CustomerResourceFilterCustomerFilter', graphql_name='customer')
+    environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
+    or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilter')), graphql_name='or')
+    resource_id = sgqlc.types.Field('StringFieldComparison', graphql_name='resourceId')
+    subscriptions = sgqlc.types.Field('CustomerResourceFilterCustomerSubscriptionFilter', graphql_name='subscriptions')
+
+
+class CustomerResourceFilterCustomerFilter(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('and_', 'billing_id', 'created_at', 'crm_hubspot_company_id', 'crm_hubspot_company_url', 'crm_id', 'customer_id', 'email', 'environment_id', 'id', 'name', 'or_', 'ref_id', 'updated_at')
+    and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilterCustomerFilter')), graphql_name='and')
+    billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
+    created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
+    crm_hubspot_company_id = sgqlc.types.Field('StringFieldComparison', graphql_name='crmHubspotCompanyId')
+    crm_hubspot_company_url = sgqlc.types.Field('StringFieldComparison', graphql_name='crmHubspotCompanyUrl')
+    crm_id = sgqlc.types.Field('StringFieldComparison', graphql_name='crmId')
+    customer_id = sgqlc.types.Field('StringFieldComparison', graphql_name='customerId')
+    email = sgqlc.types.Field('StringFieldComparison', graphql_name='email')
+    environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
+    id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
+    name = sgqlc.types.Field('StringFieldComparison', graphql_name='name')
+    or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilterCustomerFilter')), graphql_name='or')
+    ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
+    updated_at = sgqlc.types.Field('DateFieldComparison', graphql_name='updatedAt')
+
+
+class CustomerResourceFilterCustomerSubscriptionFilter(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilterCustomerSubscriptionFilter')), graphql_name='and')
+    billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
+    cancel_reason = sgqlc.types.Field('SubscriptionCancelReasonFilterComparison', graphql_name='cancelReason')
+    cancellation_date = sgqlc.types.Field('DateFieldComparison', graphql_name='cancellationDate')
+    created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
+    crm_id = sgqlc.types.Field('StringFieldComparison', graphql_name='crmId')
+    crm_link_url = sgqlc.types.Field('StringFieldComparison', graphql_name='crmLinkUrl')
+    effective_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='effectiveEndDate')
+    end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='endDate')
+    environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
+    id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
+    old_billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='oldBillingId')
+    or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilterCustomerSubscriptionFilter')), graphql_name='or')
+    pricing_type = sgqlc.types.Field('PricingTypeFilterComparison', graphql_name='pricingType')
+    ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
+    start_date = sgqlc.types.Field('DateFieldComparison', graphql_name='startDate')
+    status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
+    subscription_id = sgqlc.types.Field('StringFieldComparison', graphql_name='subscriptionId')
+    trial_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='trialEndDate')
+
+
+class CustomerResourceSort(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('direction', 'field', 'nulls')
+    direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
+    field = sgqlc.types.Field(sgqlc.types.non_null(CustomerResourceSortFields), graphql_name='field')
+    nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
+
+
 class CustomerSort(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('direction', 'field', 'nulls')
     direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
     field = sgqlc.types.Field(sgqlc.types.non_null(CustomerSortFields), graphql_name='field')
     nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
 
@@ -1459,23 +1532,31 @@
 class HubspotCredentialsInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('authorization_code', 'refresh_token')
     authorization_code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='authorizationCode')
     refresh_token = sgqlc.types.Field(String, graphql_name='refreshToken')
 
 
+class ImportCustomerBulk(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('customers', 'environment_id')
+    customers = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('ImportCustomerInput'))), graphql_name='customers')
+    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
+
+
 class ImportCustomerInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'billing_id', 'customer_id', 'email', 'environment_id', 'name', 'ref_id')
+    __field_names__ = ('additional_meta_data', 'billing_id', 'customer_id', 'email', 'environment_id', 'name', 'payment_method_id', 'ref_id')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
-    billing_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='billingId')
+    billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     customer_id = sgqlc.types.Field(String, graphql_name='customerId')
     email = sgqlc.types.Field(String, graphql_name='email')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     name = sgqlc.types.Field(String, graphql_name='name')
+    payment_method_id = sgqlc.types.Field(String, graphql_name='paymentMethodId')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
 
 
 class ImportIntegrationCatalogInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('billing_model', 'entity_selection_mode', 'environment_id', 'feature_unit_name', 'feature_unit_plural_name', 'plans_selection_blacklist', 'plans_selection_whitelist', 'product_id', 'selected_addon_billing_ids', 'vendor_identifier')
     billing_model = sgqlc.types.Field(BillingModel, graphql_name='billingModel')
@@ -1517,14 +1598,34 @@
     __schema__ = schema
     __field_names__ = ('direction', 'field', 'nulls')
     direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
     field = sgqlc.types.Field(sgqlc.types.non_null(ImportIntegrationTaskSortFields), graphql_name='field')
     nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
 
 
+class ImportSubscriptionInput(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('additional_meta_data', 'billing_id', 'billing_period', 'customer_id', 'plan_id', 'resource_id', 'start_date', 'unit_quantity')
+    additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
+    billing_id = sgqlc.types.Field(String, graphql_name='billingId')
+    billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
+    customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
+    plan_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='planId')
+    resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
+    start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
+    unit_quantity = sgqlc.types.Field(Float, graphql_name='unitQuantity')
+
+
+class ImportSubscriptionsBulk(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('environment_id', 'subscriptions')
+    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
+    subscriptions = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ImportSubscriptionInput))), graphql_name='subscriptions')
+
+
 class InitAddStripeCustomerPaymentMethodInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('customer_ref_id', 'environment_id')
     customer_ref_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerRefId')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
 
 
@@ -2989,20 +3090,21 @@
     resource_ref_id = sgqlc.types.Field(String, graphql_name='resourceRefId')
     start_date = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='startDate')
     weekly_reset_period_configuration = sgqlc.types.Field('WeeklyResetPeriodConfigInput', graphql_name='weeklyResetPeriodConfiguration')
 
 
 class UsageMeasurementCreateInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('created_at', 'customer_id', 'environment_id', 'feature_id', 'resource_id', 'value')
+    __field_names__ = ('created_at', 'customer_id', 'environment_id', 'feature_id', 'resource_id', 'update_behavior', 'value')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     feature_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='featureId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
+    update_behavior = sgqlc.types.Field(UsageUpdateBehavior, graphql_name='updateBehavior')
     value = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='value')
 
 
 class UsageMeasurementFilter(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('and_', 'created_at', 'customer', 'environment_id', 'feature', 'id', 'or_')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('UsageMeasurementFilter')), graphql_name='and')
@@ -3456,15 +3558,15 @@
     __schema__ = schema
     __field_names__ = ('id',)
     id = sgqlc.types.Field(Float, graphql_name='id')
 
 
 class Customer(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'billing_currency', 'billing_id', 'billing_link_url', 'coupon', 'created_at', 'crm_hubspot_company_id', 'crm_hubspot_company_url', 'crm_id', 'customer_id', 'default_payment_expiration_month', 'default_payment_expiration_year', 'default_payment_method_id', 'default_payment_method_last4_digits', 'default_payment_method_type', 'eligible_for_trial', 'email', 'environment', 'environment_id', 'exclude_from_experiment', 'experiment', 'experiment_info', 'has_active_subscription', 'has_payment_method', 'id', 'name', 'promotional_entitlements', 'ref_id', 'subscriptions', 'sync_states', 'trialed_plans', 'updated_at')
+    __field_names__ = ('additional_meta_data', 'billing_currency', 'billing_id', 'billing_link_url', 'coupon', 'created_at', 'crm_hubspot_company_id', 'crm_hubspot_company_url', 'crm_id', 'customer_id', 'default_payment_expiration_month', 'default_payment_expiration_year', 'default_payment_method_id', 'default_payment_method_last4_digits', 'default_payment_method_type', 'eligible_for_trial', 'email', 'environment', 'environment_id', 'exclude_from_experiment', 'experiment', 'experiment_info', 'has_active_resource', 'has_active_subscription', 'has_payment_method', 'id', 'name', 'promotional_entitlements', 'ref_id', 'subscriptions', 'sync_states', 'total_active_subscription', 'trialed_plans', 'updated_at')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     billing_currency = sgqlc.types.Field(Currency, graphql_name='billingCurrency')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_link_url = sgqlc.types.Field(String, graphql_name='billingLinkUrl')
     coupon = sgqlc.types.Field(Coupon, graphql_name='coupon')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_hubspot_company_id = sgqlc.types.Field(String, graphql_name='crmHubspotCompanyId')
@@ -3479,14 +3581,15 @@
     eligible_for_trial = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('EligibleForTrial')), graphql_name='eligibleForTrial')
     email = sgqlc.types.Field(String, graphql_name='email')
     environment = sgqlc.types.Field('Environment', graphql_name='environment')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
     exclude_from_experiment = sgqlc.types.Field(Boolean, graphql_name='excludeFromExperiment')
     experiment = sgqlc.types.Field('Experiment', graphql_name='experiment')
     experiment_info = sgqlc.types.Field('experimentInfo', graphql_name='experimentInfo')
+    has_active_resource = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasActiveResource')
     has_active_subscription = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasActiveSubscription')
     has_payment_method = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasPaymentMethod')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     name = sgqlc.types.Field(String, graphql_name='name')
     promotional_entitlements = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('PromotionalEntitlement'))), graphql_name='promotionalEntitlements', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(PromotionalEntitlementFilter, graphql_name='filter', default={})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(PromotionalEntitlementSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
@@ -3495,14 +3598,15 @@
     ref_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='refId')
     subscriptions = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscription')), graphql_name='subscriptions', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(CustomerSubscriptionFilter, graphql_name='filter', default={'status': {'in': ['ACTIVE', 'IN_TRIAL']}})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(CustomerSubscriptionSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     sync_states = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SyncState')), graphql_name='syncStates')
+    total_active_subscription = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='totalActiveSubscription')
     trialed_plans = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('TrialedPlan')), graphql_name='trialedPlans')
     updated_at = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='updatedAt')
 
 
 class CustomerAggregateGroupBy(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('billing_id', 'created_at', 'crm_hubspot_company_id', 'crm_hubspot_company_url', 'crm_id', 'customer_id', 'email', 'environment_id', 'id', 'name', 'ref_id', 'updated_at')
@@ -3705,16 +3809,71 @@
     pricing_type = sgqlc.types.Field(sgqlc.types.non_null(PricingType), graphql_name='pricingType')
     unit_quantity = sgqlc.types.Field(Int, graphql_name='unitQuantity')
     usage_based_estimated_bill = sgqlc.types.Field(Float, graphql_name='usageBasedEstimatedBill')
 
 
 class CustomerResource(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('resource_id',)
+    __field_names__ = ('created_at', 'customer', 'environment_id', 'resource_id', 'subscriptions')
+    created_at = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='createdAt')
+    customer = sgqlc.types.Field(sgqlc.types.non_null(Customer), graphql_name='customer')
+    environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
     resource_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='resourceId')
+    subscriptions = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscription'))), graphql_name='subscriptions', args=sgqlc.types.ArgDict((
+        ('filter', sgqlc.types.Arg(CustomerSubscriptionFilter, graphql_name='filter', default={'status': {'in': ['ACTIVE', 'IN_TRIAL']}})),
+        ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(CustomerSubscriptionSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
+))
+    )
+
+
+class CustomerResourceAggregateGroupBy(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('created_at', 'environment_id', 'resource_id')
+    created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
+    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
+    resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
+
+
+class CustomerResourceConnection(sgqlc.types.relay.Connection):
+    __schema__ = schema
+    __field_names__ = ('edges', 'page_info', 'total_count')
+    edges = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceEdge'))), graphql_name='edges')
+    page_info = sgqlc.types.Field(sgqlc.types.non_null('PageInfo'), graphql_name='pageInfo')
+    total_count = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='totalCount')
+
+
+class CustomerResourceCountAggregate(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('created_at', 'environment_id', 'resource_id')
+    created_at = sgqlc.types.Field(Int, graphql_name='createdAt')
+    environment_id = sgqlc.types.Field(Int, graphql_name='environmentId')
+    resource_id = sgqlc.types.Field(Int, graphql_name='resourceId')
+
+
+class CustomerResourceEdge(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('cursor', 'node')
+    cursor = sgqlc.types.Field(sgqlc.types.non_null(ConnectionCursor), graphql_name='cursor')
+    node = sgqlc.types.Field(sgqlc.types.non_null(CustomerResource), graphql_name='node')
+
+
+class CustomerResourceMaxAggregate(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('created_at', 'environment_id', 'resource_id')
+    created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
+    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
+    resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
+
+
+class CustomerResourceMinAggregate(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('created_at', 'environment_id', 'resource_id')
+    created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
+    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
+    resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
 
 
 class CustomerSubscription(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('additional_meta_data', 'addons', 'billing_id', 'billing_link_url', 'cancel_reason', 'cancellation_date', 'coupon', 'created_at', 'crm_id', 'crm_link_url', 'current_billing_period_end', 'customer', 'effective_end_date', 'end_date', 'environment', 'environment_id', 'experiment', 'experiment_info', 'id', 'is_custom_price_subscription', 'old_billing_id', 'outdated_price_packages', 'plan', 'prices', 'pricing_type', 'ref_id', 'resource', 'resource_id', 'scheduled_updates', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'sync_states', 'total_price', 'trial_end_date', 'was_in_trial')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddon')), graphql_name='addons', args=sgqlc.types.ArgDict((
@@ -4803,15 +4962,15 @@
     __schema__ = schema
     __field_names__ = ('monthly_according_to',)
     monthly_according_to = sgqlc.types.Field(MonthlyAccordingTo, graphql_name='monthlyAccordingTo')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('add_compatible_addons_to_plan', 'archive_one_coupon', 'archive_plan', 'attach_customer_payment_method', 'cancel_schedule', 'cancel_subscription', 'create_account', 'create_addon_draft', 'create_feature', 'create_many_package_entitlements', 'create_many_promotional_entitlements', 'create_one_addon', 'create_one_coupon', 'create_one_customer', 'create_one_environment', 'create_one_experiment', 'create_one_feature', 'create_one_hook', 'create_one_integration', 'create_one_plan', 'create_one_product', 'create_plan_draft', 'create_subscription', 'create_usage_measurement', 'delete_environment', 'delete_feature', 'delete_one_addon', 'delete_one_customer', 'delete_one_environment', 'delete_one_feature', 'delete_one_hook', 'delete_one_integration', 'delete_one_package_entitlement', 'delete_one_price', 'delete_one_product', 'delete_one_promotional_entitlement', 'estimate_subscription', 'estimate_subscription_update', 'hide_getting_started_page', 'import_one_customer', 'init_add_stripe_customer_payment_method', 'initiate_checkout', 'invite_members', 'migrate_subscription_to_latest', 'provision_customer', 'provision_sandbox', 'provision_subscription', 'provision_subscription_v2', 'publish_addon', 'publish_plan', 'purge_customer_cache', 'register_member', 'remove_addon_draft', 'remove_base_plan_from_plan', 'remove_compatible_addons_from_plan', 'remove_coupon_from_customer', 'remove_coupon_from_customer_subscription', 'remove_experiment_from_customer', 'remove_experiment_from_customer_subscription', 'remove_member', 'remove_plan_draft', 'report_entitlement_check_requested', 'resend_email_verification', 'resync_integration', 'set_base_plan_on_plan', 'set_compatible_addons_on_plan', 'set_coupon_on_customer', 'set_coupon_on_customer_subscription', 'set_experiment_on_customer', 'set_experiment_on_customer_subscription', 'set_package_pricing', 'set_widget_configuration', 'start_experiment', 'stop_experiment', 'trigger_import_catalog', 'trigger_import_customers', 'update_account', 'update_entitlements_order', 'update_feature', 'update_one_addon', 'update_one_coupon', 'update_one_customer', 'update_one_environment', 'update_one_experiment', 'update_one_feature', 'update_one_hook', 'update_one_integration', 'update_one_package_entitlement', 'update_one_plan', 'update_one_product', 'update_one_promotional_entitlement', 'update_one_subscription', 'update_user')
+    __field_names__ = ('add_compatible_addons_to_plan', 'archive_one_coupon', 'archive_plan', 'attach_customer_payment_method', 'cancel_schedule', 'cancel_subscription', 'create_account', 'create_addon_draft', 'create_feature', 'create_many_package_entitlements', 'create_many_promotional_entitlements', 'create_one_addon', 'create_one_coupon', 'create_one_customer', 'create_one_environment', 'create_one_experiment', 'create_one_feature', 'create_one_hook', 'create_one_integration', 'create_one_plan', 'create_one_product', 'create_plan_draft', 'create_subscription', 'create_usage_measurement', 'delete_environment', 'delete_feature', 'delete_one_addon', 'delete_one_customer', 'delete_one_environment', 'delete_one_feature', 'delete_one_hook', 'delete_one_integration', 'delete_one_package_entitlement', 'delete_one_price', 'delete_one_product', 'delete_one_promotional_entitlement', 'estimate_subscription', 'estimate_subscription_update', 'hide_getting_started_page', 'import_customers_bulk', 'import_one_customer', 'import_subscriptions_bulk', 'init_add_stripe_customer_payment_method', 'initiate_checkout', 'invite_members', 'migrate_subscription_to_latest', 'provision_customer', 'provision_sandbox', 'provision_subscription', 'provision_subscription_v2', 'publish_addon', 'publish_plan', 'purge_customer_cache', 'register_member', 'remove_addon_draft', 'remove_base_plan_from_plan', 'remove_compatible_addons_from_plan', 'remove_coupon_from_customer', 'remove_coupon_from_customer_subscription', 'remove_experiment_from_customer', 'remove_experiment_from_customer_subscription', 'remove_member', 'remove_plan_draft', 'report_entitlement_check_requested', 'resend_email_verification', 'resync_integration', 'set_base_plan_on_plan', 'set_compatible_addons_on_plan', 'set_coupon_on_customer', 'set_coupon_on_customer_subscription', 'set_experiment_on_customer', 'set_experiment_on_customer_subscription', 'set_package_pricing', 'set_widget_configuration', 'start_experiment', 'stop_experiment', 'trigger_import_catalog', 'trigger_import_customers', 'update_account', 'update_entitlements_order', 'update_feature', 'update_one_addon', 'update_one_coupon', 'update_one_customer', 'update_one_environment', 'update_one_experiment', 'update_one_feature', 'update_one_hook', 'update_one_integration', 'update_one_package_entitlement', 'update_one_plan', 'update_one_product', 'update_one_promotional_entitlement', 'update_one_subscription', 'update_user')
     add_compatible_addons_to_plan = sgqlc.types.Field(sgqlc.types.non_null('Plan'), graphql_name='addCompatibleAddonsToPlan', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(AddCompatibleAddonsToPlanInput), graphql_name='input', default=None)),
 ))
     )
     archive_one_coupon = sgqlc.types.Field(sgqlc.types.non_null(Coupon), graphql_name='archiveOneCoupon', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(ArchiveCouponInput), graphql_name='input', default=None)),
 ))
@@ -4960,18 +5119,26 @@
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(EstimateSubscriptionUpdateInput), graphql_name='input', default=None)),
 ))
     )
     hide_getting_started_page = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='hideGettingStartedPage', args=sgqlc.types.ArgDict((
         ('member_id', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='memberId', default=None)),
 ))
     )
+    import_customers_bulk = sgqlc.types.Field(String, graphql_name='importCustomersBulk', args=sgqlc.types.ArgDict((
+        ('input', sgqlc.types.Arg(sgqlc.types.non_null(ImportCustomerBulk), graphql_name='input', default=None)),
+))
+    )
     import_one_customer = sgqlc.types.Field(sgqlc.types.non_null(Customer), graphql_name='importOneCustomer', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(ImportCustomerInput), graphql_name='input', default=None)),
 ))
     )
+    import_subscriptions_bulk = sgqlc.types.Field(String, graphql_name='importSubscriptionsBulk', args=sgqlc.types.ArgDict((
+        ('input', sgqlc.types.Arg(sgqlc.types.non_null(ImportSubscriptionsBulk), graphql_name='input', default=None)),
+))
+    )
     init_add_stripe_customer_payment_method = sgqlc.types.Field(sgqlc.types.non_null(InitAddStripeCustomerPaymentMethod), graphql_name='initAddStripeCustomerPaymentMethod', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(InitAddStripeCustomerPaymentMethodInput), graphql_name='input', default=None)),
 ))
     )
     initiate_checkout = sgqlc.types.Field(sgqlc.types.non_null(Checkout), graphql_name='initiateCheckout', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(InitiateCheckoutInput), graphql_name='input', default=None)),
 ))
@@ -6042,15 +6209,15 @@
     __schema__ = schema
     __field_names__ = ('task_id',)
     task_id = sgqlc.types.Field(String, graphql_name='taskId')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('addons', 'cached_entitlements', 'coupon', 'coupons', 'current_environment', 'current_user', 'customer_portal', 'customer_subscriptions', 'customers', 'entitlement', 'entitlements', 'environments', 'experiment', 'experiments', 'features', 'fetch_account', 'get_active_subscriptions', 'get_addon_by_ref_id', 'get_customer_by_ref_id', 'get_experiment_stats', 'get_paywall', 'get_plan_by_ref_id', 'hook', 'hooks', 'import_integration_tasks', 'integrations', 'members', 'mock_paywall', 'package_entitlements', 'paywall', 'plans', 'products', 'promotional_entitlements', 'sdk_configuration', 'send_test_hook', 'stripe_customers', 'stripe_products', 'stripe_subscriptions', 'subscription_entitlements', 'subscription_migration_tasks', 'test_hook_data', 'usage_history', 'usage_measurements', 'widget_configuration')
+    __field_names__ = ('addons', 'cached_entitlements', 'coupon', 'coupons', 'current_environment', 'current_user', 'customer_portal', 'customer_resources', 'customer_subscriptions', 'customers', 'entitlement', 'entitlements', 'environments', 'experiment', 'experiments', 'features', 'fetch_account', 'get_active_subscriptions', 'get_addon_by_ref_id', 'get_customer_by_ref_id', 'get_experiment_stats', 'get_paywall', 'get_plan_by_ref_id', 'hook', 'hooks', 'import_integration_tasks', 'integrations', 'members', 'mock_paywall', 'package_entitlements', 'paywall', 'plans', 'products', 'promotional_entitlements', 'sdk_configuration', 'send_test_hook', 'stripe_customers', 'stripe_products', 'stripe_subscriptions', 'subscription_entitlements', 'subscription_migration_tasks', 'test_hook_data', 'usage_history', 'usage_measurements', 'widget_configuration')
     addons = sgqlc.types.Field(sgqlc.types.non_null(AddonConnection), graphql_name='addons', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(AddonFilter, graphql_name='filter', default={})),
         ('paging', sgqlc.types.Arg(CursorPaging, graphql_name='paging', default={'first': 10})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(AddonSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     cached_entitlements = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Entitlement))), graphql_name='cachedEntitlements', args=sgqlc.types.ArgDict((
@@ -6069,14 +6236,20 @@
     )
     current_environment = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='currentEnvironment')
     current_user = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='currentUser')
     customer_portal = sgqlc.types.Field(sgqlc.types.non_null(CustomerPortal), graphql_name='customerPortal', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(CustomerPortalInput), graphql_name='input', default=None)),
 ))
     )
+    customer_resources = sgqlc.types.Field(sgqlc.types.non_null(CustomerResourceConnection), graphql_name='customerResources', args=sgqlc.types.ArgDict((
+        ('filter', sgqlc.types.Arg(CustomerResourceFilter, graphql_name='filter', default={})),
+        ('paging', sgqlc.types.Arg(CursorPaging, graphql_name='paging', default={'first': 10})),
+        ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(CustomerResourceSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
+))
+    )
     customer_subscriptions = sgqlc.types.Field(sgqlc.types.non_null(CustomerSubscriptionConnection), graphql_name='customerSubscriptions', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(CustomerSubscriptionFilter, graphql_name='filter', default={})),
         ('paging', sgqlc.types.Arg(CursorPaging, graphql_name='paging', default={'first': 10})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(CustomerSubscriptionSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     customers = sgqlc.types.Field(sgqlc.types.non_null(CustomerConnection), graphql_name='customers', args=sgqlc.types.ArgDict((
```

### Comparing `stigg_api_client-0.4.0/PKG-INFO` & `stigg_api_client-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

