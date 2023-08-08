# Comparing `tmp/bitpay-3.4.2203.tar.gz` & `tmp/bitpay-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitpay-3.4.2203.tar", last modified: Mon Mar 14 09:10:15 2022, max compression
+gzip compressed data, was "bitpay-4.0.0.tar", last modified: Tue Aug  8 23:41:38 2023, max compression
```

## Comparing `bitpay-3.4.2203.tar` & `bitpay-4.0.0.tar`

### file list

```diff
@@ -1,143 +1,139 @@
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1760 2022-03-14 09:10:15.000000 bitpay-3.4.2203/PKG-INFO
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     2796 2022-03-08 15:38:16.000000 bitpay-3.4.2203/README.md
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1907 2022-03-14 09:10:02.000000 bitpay-3.4.2203/setup.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)       79 2022-03-14 09:10:15.000000 bitpay-3.4.2203/setup.cfg
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      853 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/config.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      231 2022-03-14 09:10:02.000000 bitpay-3.4.2203/src/bitpay/env.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)    69834 2022-03-14 09:10:02.000000 bitpay-3.4.2203/src/bitpay/client.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/__init__.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/utils/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/utils/__init__.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     2183 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/utils/key_utils.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     5017 2022-03-14 09:06:08.000000 bitpay-3.4.2203/src/bitpay/utils/rest_cli.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     2711 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/tokens.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/models/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      107 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/facade.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/models/Rate/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1449 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/Rate/rate.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/Rate/__init__.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1873 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/Rate/rates.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/models/ledger/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     4034 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/ledger/buyer.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1569 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/ledger/ledger.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/ledger/__init__.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     7168 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/ledger/ledger_entry.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/models/bill/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     9877 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/bill/bill.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      170 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/bill/bill_status.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/bill/__init__.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1923 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/bill/item.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/models/settlement/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     2679 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/settlement/with_holdings.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     3625 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/settlement/settlement_ledger_entry.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     9487 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/settlement/settlement.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/settlement/__init__.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1802 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/settlement/refund_info.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     5376 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/settlement/invoice_data.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)    10825 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/settlement/payout_info.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/__init__.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/models/subscription/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     3861 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/subscription/subscription.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     7701 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/subscription/bill_data.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/subscription/__init__.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      166 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/subscription/subscription_status.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1765 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/subscription/item.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/models/wallet/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/wallet/__init__.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     3477 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/wallet/currencies.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1178 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/wallet/currency_qr.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     2841 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/wallet/wallet.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     9354 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/currency.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/models/payout/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      235 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/recipient_status.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     2374 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout_recipients.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1639 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout_received_info.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      227 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout_status.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1983 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout_instruction_transaction.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)    12941 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1950 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout_transaction.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/__init__.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     3889 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout_recipient.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)    13908 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout_batch.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     2813 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout_received_info_address.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      167 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/recipient_reference_method.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     6911 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout_instruction.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1305 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/payout/payout_instruction_btc_summary.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/models/invoice/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     3139 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/buyer_provided_info.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      217 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/invoice_status.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     4653 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/buyer.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     4077 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/refund_params.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      786 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/shopper.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/__init__.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1755 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/itemized_details.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     4700 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/supported_transaction_currencies.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1250 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/supported_transaction_currency.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     4349 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/miner_fees.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      226 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/refund_status.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1735 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/refund_info.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1582 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/universal_codes.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     7849 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/refund.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)    31918 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/invoice.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     2159 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/models/invoice/miner_fees_item.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay/exceptions/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      814 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      797 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/rate_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      805 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/bill_creation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      878 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      833 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/currency_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      910 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/currency_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      865 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/bill_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      875 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_recipient_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      865 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payoutbatch_cancellation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      802 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/refund_update_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      814 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/refund_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      834 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_cancellation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      921 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_recipient_cancellation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      837 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/refund_creation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      861 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/invoice_notification_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      824 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/invoice_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      936 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/subscription_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      866 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/rates_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      835 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/invoice_creation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      923 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/settlement_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      852 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payoutbatch_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        0 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/__init__.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      835 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/refund_cancellation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      814 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/ledger_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      782 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/bill_update_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      887 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/subscription_creation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      862 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/subscription_update_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      879 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/ledger_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      858 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payoutbatch_creation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      956 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_recipient_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      856 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/settlement_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      884 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payoutbatch_notification_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      825 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_creation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      852 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_notification_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      808 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/bill_delivery_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      935 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_recipient_notification_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      878 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/refund_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      812 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/invoice_update_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      932 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payoutbatch_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      844 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/invoice_cancellation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      911 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_recipient_creation_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      902 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/bitpay_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      794 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/bill_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      815 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/invoice_payment_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      874 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/subscription_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      852 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/refund_notification_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      885 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/invoice_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      888 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/payout_recipient_update_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      878 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/wallet_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)      815 2022-03-08 15:38:16.000000 bitpay-3.4.2203/src/bitpay/exceptions/wallet_query_exception.py
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     6024 2022-03-09 14:50:19.000000 bitpay-3.4.2203/src/bitpay/bitpay_setup.py
-drwxr-xr-x   0 antonio.buedo   (501) staff       (20)        0 2022-03-14 09:10:15.000000 bitpay-3.4.2203/src/bitpay.egg-info/
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     1760 2022-03-14 09:10:14.000000 bitpay-3.4.2203/src/bitpay.egg-info/PKG-INFO
--rw-r--r--   0 antonio.buedo   (501) staff       (20)     5470 2022-03-14 09:10:14.000000 bitpay-3.4.2203/src/bitpay.egg-info/SOURCES.txt
--rw-r--r--   0 antonio.buedo   (501) staff       (20)       15 2022-03-14 09:10:14.000000 bitpay-3.4.2203/src/bitpay.egg-info/requires.txt
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        7 2022-03-14 09:10:14.000000 bitpay-3.4.2203/src/bitpay.egg-info/top_level.txt
--rw-r--r--   0 antonio.buedo   (501) staff       (20)        1 2022-03-14 09:10:14.000000 bitpay-3.4.2203/src/bitpay.egg-info/dependency_links.txt
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.590327 bitpay-4.0.0/
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1063 2023-04-12 21:49:08.000000 bitpay-4.0.0/LICENSE
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1599 2023-08-08 23:41:38.590385 bitpay-4.0.0/PKG-INFO
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1810 2023-08-07 03:44:53.000000 bitpay-4.0.0/README.md
+-rw-r--r--   0 r.brodie   (501) staff       (20)      251 2023-08-08 23:41:38.590597 bitpay-4.0.0/setup.cfg
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1860 2023-08-07 13:49:02.000000 bitpay-4.0.0/setup.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.575281 bitpay-4.0.0/src/
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.576928 bitpay-4.0.0/src/bitpay/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     6205 2023-08-08 21:58:03.000000 bitpay-4.0.0/src/bitpay/bitpay_setup.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)    36304 2023-08-08 21:54:53.000000 bitpay-4.0.0/src/bitpay/client.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.579040 bitpay-4.0.0/src/bitpay/clients/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     6303 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/bill_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     5477 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/bitpay_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1423 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/currency_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)    16611 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/invoice_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     3165 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/ledger_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     9177 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/payout_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     9073 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/payout_recipient_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     3886 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/rate_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)    13422 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/refund_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     5221 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/settlement_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1448 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/clients/wallet_client.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      279 2023-08-07 03:45:24.000000 bitpay-4.0.0/src/bitpay/config.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)       85 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/environment.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.583980 bitpay-4.0.0/src/bitpay/exceptions/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/exceptions/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      824 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/bill_creation_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      827 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/bill_delivery_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      886 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/bill_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      813 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/bill_query_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      801 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/bill_update_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      928 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/bitpay_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      931 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/currency_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      852 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/currency_query_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      863 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/invoice_cancellation_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      854 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/invoice_creation_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      906 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/invoice_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      880 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/invoice_notification_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      834 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/invoice_payment_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      843 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/invoice_query_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      831 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/invoice_update_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      900 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/ledger_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      833 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/ledger_query_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      853 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_cancellation_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      844 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_creation_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      899 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      871 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_notification_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      833 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_query_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      940 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_cancellation_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      930 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_creation_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      977 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      954 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_notification_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      894 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_query_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      907 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_update_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      816 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/rate_query_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      887 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/rates_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      854 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/refund_cancellation_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      856 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/refund_creation_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      899 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/refund_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      871 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/refund_notification_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      833 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/refund_query_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      821 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/refund_update_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      944 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/settlement_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      875 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/settlement_query_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      899 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/wallet_exception.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      834 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/exceptions/wallet_query_exception.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.584315 bitpay-4.0.0/src/bitpay/models/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/__init__.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.584739 bitpay-4.0.0/src/bitpay/models/bill/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/bill/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     9201 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/bill/bill.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      170 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/bill/bill_status.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     2155 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/bill/item.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     7594 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/currency.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      215 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/facade.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.586804 bitpay-4.0.0/src/bitpay/models/invoice/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/invoice/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     4742 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/buyer.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     3883 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/buyer_provided_info.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)    32718 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/invoice.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1167 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/invoice_event_token.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      217 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/invoice/invoice_status.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1896 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/itemized_details.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     4335 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/miner_fees.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     2493 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/miner_fees_item.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)    10046 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/refund.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1932 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/refund_info.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      226 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/invoice/refund_status.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      905 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/shopper.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     5024 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/supported_transaction_currencies.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1436 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/supported_transaction_currency.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     2123 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/transaction.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1569 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/invoice/universal_codes.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.587221 bitpay-4.0.0/src/bitpay/models/ledger/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/ledger/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     4079 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/ledger/buyer.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1428 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/ledger/ledger.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     6776 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/ledger/ledger_entry.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.588266 bitpay-4.0.0/src/bitpay/models/payout/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/payout/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)    11788 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/payout/payout.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      727 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/payout/payout_group.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1058 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/payout/payout_group_failed.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     4051 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/payout/payout_recipient.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1908 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/payout/payout_recipients.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      227 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/payout/payout_status.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     2177 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/payout/payout_transaction.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      235 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/payout/recipient_status.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.588561 bitpay-4.0.0/src/bitpay/models/rate/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/rate/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1640 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/rate/rate.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1167 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/rate/rates.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.589288 bitpay-4.0.0/src/bitpay/models/settlement/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/settlement/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     4986 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/settlement/invoice_data.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)    10814 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/settlement/payout_info.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     2380 2023-08-08 21:54:53.000000 bitpay-4.0.0/src/bitpay/models/settlement/refund_info.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     8730 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/settlement/settlement.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     3797 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/settlement/settlement_ledger_entry.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     2840 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/settlement/with_holdings.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.589711 bitpay-4.0.0/src/bitpay/models/wallet/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/models/wallet/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     4110 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/wallet/currencies.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1393 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/wallet/currency_qr.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     3135 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/models/wallet/wallet.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.590216 bitpay-4.0.0/src/bitpay/utils/
+-rw-r--r--   0 r.brodie   (501) staff       (20)        0 2023-04-12 21:49:08.000000 bitpay-4.0.0/src/bitpay/utils/__init__.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      104 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/utils/guid_generator.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     2367 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/utils/key_utils.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)     3795 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/utils/model_util.py
+-rw-r--r--   0 r.brodie   (501) staff       (20)      806 2023-08-07 02:34:09.000000 bitpay-4.0.0/src/bitpay/utils/token_container.py
+drwxr-xr-x   0 r.brodie   (501) staff       (20)        0 2023-08-08 23:41:38.577475 bitpay-4.0.0/src/bitpay.egg-info/
+-rw-r--r--   0 r.brodie   (501) staff       (20)     1599 2023-08-08 23:41:38.000000 bitpay-4.0.0/src/bitpay.egg-info/PKG-INFO
+-rw-r--r--   0 r.brodie   (501) staff       (20)     5030 2023-08-08 23:41:38.000000 bitpay-4.0.0/src/bitpay.egg-info/SOURCES.txt
+-rw-r--r--   0 r.brodie   (501) staff       (20)        1 2023-08-08 23:41:38.000000 bitpay-4.0.0/src/bitpay.egg-info/dependency_links.txt
+-rw-r--r--   0 r.brodie   (501) staff       (20)       15 2023-08-08 23:41:38.000000 bitpay-4.0.0/src/bitpay.egg-info/requires.txt
+-rw-r--r--   0 r.brodie   (501) staff       (20)        7 2023-08-08 23:41:38.000000 bitpay-4.0.0/src/bitpay.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bitpay-3.4.2203/PKG-INFO` & `bitpay-4.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: bitpay
-Version: 3.4.2203
+Version: 4.0.0
 Summary: Accept bitcoin with BitPay
 Home-page: https://github.com/bitpay/python-bitpay-client
+Download-URL: https://github.com/bitpay/python-bitpay-client/tarball/v3.4.2203
 Author: Antonio Buedo
 Author-email: sales-engineering@bitpay.com
-License: UNKNOWN
-Download-URL: https://github.com/bitpay/python-bitpay-client/tarball/v3.4.2203
-Description:         Python Library for integrating with BitPay
-                
-                This library is a simple way to integrate your application with
-                BitPay for taking Bitcoin payments. It exposes three basic 
-                functions, authenticating with BitPay, creating invoices, 
-                and retrieving invoices. It is not meant as a replacement for 
-                the entire BitPay API. However, the key_utils module contains
-                all of the tools you need to use the BitPay API for other
-                purposes.
-                
-                This version requires only Python 3.8.
-                
 Keywords: bitcoin,payments,crypto,cash,ethereum,online payments
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Office/Business :: Financial
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+        Python Library for integrating with BitPay
+        
+        This library is a simple way to integrate your application with
+        BitPay for taking Bitcoin payments. It exposes three basic 
+        functions, authenticating with BitPay, creating invoices, 
+        and retrieving invoices. It is not meant as a replacement for 
+        the entire BitPay API. However, the key_utils module contains
+        all of the tools you need to use the BitPay API for other
+        purposes.
+        
+        This version requires Python 3.8 or higher.
+
```

### Comparing `bitpay-3.4.2203/setup.py` & `bitpay-4.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 """
 import setuptools
 
 setuptools.setup(
     name="bitpay",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    version="3.4.2203",
+    version="4.0.0",
     description="Accept bitcoin with BitPay",
     author="Antonio Buedo",
     author_email="sales-engineering@bitpay.com",
     url="https://github.com/bitpay/python-bitpay-client",
     download_url="https://github.com/bitpay/python-bitpay-client/tarball/v3.4.2203",
     keywords=["bitcoin", "payments", "crypto", "cash", "ethereum", "online payments"],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=["requests", "ecdsa"],
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Environment :: Web Environment",
@@ -38,11 +37,11 @@
         BitPay for taking Bitcoin payments. It exposes three basic 
         functions, authenticating with BitPay, creating invoices, 
         and retrieving invoices. It is not meant as a replacement for 
         the entire BitPay API. However, the key_utils module contains
         all of the tools you need to use the BitPay API for other
         purposes.
         
-        This version requires only Python 3.8.
+        This version requires Python 3.8 or higher.
         """,
     long_description_content_type="text/markdown",
 )
```

### Comparing `bitpay-3.4.2203/src/bitpay/utils/key_utils.py` & `bitpay-4.0.0/src/bitpay/utils/key_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 import binascii
 import hashlib
 from ecdsa import util as ecdsaUtil
 from ecdsa import SigningKey, SECP256k1
 
 
-def generate_pem():
+def generate_pem():  # type: ignore
     s_k = SigningKey.generate(curve=SECP256k1)
     pem = s_k.to_pem()
     pem = pem.decode("utf-8")
     return pem
 
 
-def get_sin_from_pem(pem):
+def get_sin_from_pem(pem):  # type: ignore
     public_key = get_compressed_public_key_from_pem(pem)
     version = get_version_from_compressed_key(public_key)
     checksum = get_checksum_from_version(version)
     return base58encode(version + checksum)
 
 
-def get_compressed_public_key_from_pem(pem):
+def get_compressed_public_key_from_pem(pem):  # type: ignore
     vks = SigningKey.from_pem(pem).get_verifying_key().to_string()
     bts = binascii.hexlify(vks)
     compressed = compress_key(bts)
     return compressed
 
 
-def sign(message, pem):
+def sign(message, pem):  # type: ignore
     message = message.encode()
     s_k = SigningKey.from_pem(pem)
     signed = s_k.sign(
         message, hashfunc=hashlib.sha256, sigencode=ecdsaUtil.sigencode_der
     )
     return binascii.hexlify(signed).decode()
 
 
-def base58encode(hexastring):
+def base58encode(hexastring):  # type: ignore
     chars = "123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz"
     int_val = int(hexastring, 16)
     encoded = encode58("", int_val, chars)
     return encoded
 
 
-def encode58(string, int_val, chars):
+def encode58(string, int_val, chars):  # type: ignore
     if int_val == 0:
         return string
     else:
         new_val, rem = divmod(int_val, 58)
         new_string = (chars[rem]) + string
         return encode58(new_string, new_val, chars)
 
 
-def get_checksum_from_version(version):
+def get_checksum_from_version(version):  # type: ignore
     return sha_digest(sha_digest(version))[0:8]
 
 
-def get_version_from_compressed_key(key):
+def get_version_from_compressed_key(key):  # type: ignore
     sh2 = sha_digest(key)
     rphash = hashlib.new("ripemd160")
     rphash.update(binascii.unhexlify(sh2))
     rp1 = rphash.hexdigest()
     return "0F02" + rp1
 
 
-def sha_digest(hexastring):
+def sha_digest(hexastring):  # type: ignore
     return hashlib.sha256(binascii.unhexlify(hexastring)).hexdigest()
 
 
-def compress_key(bts):
+def compress_key(bts):  # type: ignore
     intval = int(bts, 16)
     prefix = find_prefix(intval)
     return prefix + bts[0:64].decode("utf-8")
 
 
-def find_prefix(intval):
+def find_prefix(intval: int) -> str:
     if intval % 2 == 0:
         prefix = "02"
     else:
         prefix = "03"
     return prefix
 
 
-def change_camel_case_to_snake_case(string):
+def change_camel_case_to_snake_case(string: str) -> str:
     snake_case = "".join(
         ["_" + i.lower() if i.isupper() else i for i in string]
     ).lstrip("_")
     return snake_case
```

### Comparing `bitpay-3.4.2203/src/bitpay/utils/rest_cli.py` & `bitpay-4.0.0/src/bitpay/clients/bitpay_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,136 +1,148 @@
-"""
-HTTP methods
-"""
 import json
 import urllib
-import requests
-
-from .. import env
-from ..exceptions.bitpay_exception import BitPayException
-from .key_utils import get_compressed_public_key_from_pem, sign
+from typing import Dict, Any, Optional
 
+import requests
+from requests import Response
 
-class RESTcli:
-    __headers = {}
-    __baseurl = ""
-    __eckey = ""
-    __identity = ""
-    __proxy = ""
-
-    def __init__(self, environment, eckey, proxy=None):
-        self.__eckey = eckey
-        self.__baseurl = env.TESTURL if environment == env.TEST else env.PRODURL
+from bitpay.config import Config
+from bitpay.exceptions.bitpay_exception import BitPayException
+from bitpay.utils.key_utils import sign, get_compressed_public_key_from_pem
+from urllib.parse import urlparse
+
+
+class BitPayClient:
+    __headers: Dict[str, str] = {}
+    __base_url: str
+    __ec_key: Optional[str] = None
+    __proxy: Optional[str] = None
+
+    def __init__(
+        self, base_url: str, ec_key: Optional[str] = None, proxy: Optional[str] = None
+    ):
+        self.__base_url = base_url
+        self.__ec_key = ec_key
         self.__proxy = proxy
         self.init()
 
-    def init(self):
+    def init(self) -> None:
         try:
             self.__headers = {
-                "x-accept-version": env.BITPAYAPIVERSION,
-                "x-bitpay-plugin-info": env.BITPAYPLUGININFO,
-                "x-bitpay-api-frame": env.BITPAYAPIFRAME,
-                "x-bitpay-api-frame-version": env.BITPAYAPIFRAMEVERSION,
+                "x-accept-version": Config.BITPAY_API_VERSION.value,
+                "x-bitpay-plugin-info": Config.BITPAY_PLUGIN_INFO.value,
+                "x-bitpay-api-frame": Config.BITPAY_API_FRAME.value,
+                "x-bitpay-api-frame-version": Config.BITPAY_API_FRAME_VERSION.value,
                 "content-type": "application/json",
-                "X-accept-version": "2.0.0"
+                "X-accept-version": "2.0.0",
             }
-            if self.__proxy != "":
+            if self.__proxy is not None:
                 self.__headers["proxy"] = self.__proxy
 
         except BitPayException as e:
             print(e)
 
-    def post(self, uri, form_data, signature_required=True):
+    def post(
+        self, uri: str, form_data: Any = {}, signature_required: bool = True
+    ) -> dict:
         """
         :param uri: Url at which user wants to post the data
         :param form_data: the data to be posted
         :param signature_required: Signature of the full request URL concatenated
         with the request body
         :return: json response
         """
-        full_url = self.__baseurl + uri
+        full_url = self.__base_url + uri
         form_data = json.dumps(form_data)
         if signature_required:
-            self.__headers["x-signature"] = sign(full_url + form_data, self.__eckey)
-            self.__headers["x-identity"] = get_compressed_public_key_from_pem(self.__eckey)
+            self.__headers["x-signature"] = sign(full_url + form_data, self.__ec_key)
+            self.__headers["x-identity"] = get_compressed_public_key_from_pem(
+                self.__ec_key
+            )
 
         response = requests.post(full_url, data=form_data, headers=self.__headers)
         json_response = self.response_to_json_string(response)
         return json_response
 
-    def get(self, uri, parameters=None, signature_required=True):
+    def get(
+        self,
+        uri: str,
+        parameters: Optional[dict] = None,
+        signature_required: bool = True,
+    ) -> dict:
         """
 
         :param uri: Url from which user wants to get the data
         :param parameters: These are query parameters
         :param signature_required: Signature of the full request URL concatenated
         :return: json response
         """
-        full_url = self.__baseurl + uri
+        full_url = self.__base_url + uri
         if parameters is not None:
             full_url = "%s?%s" % (full_url, urllib.parse.urlencode(parameters))
 
         if signature_required:
-            self.__headers["x-signature"] = sign(full_url, self.__eckey)
-            self.__headers["x-identity"] = get_compressed_public_key_from_pem(self.__eckey)
+            self.__headers["x-signature"] = sign(full_url, self.__ec_key)
+            self.__headers["x-identity"] = get_compressed_public_key_from_pem(
+                self.__ec_key
+            )
 
         response = requests.get(full_url, headers=self.__headers)
         json_response = self.response_to_json_string(response)
         return json_response
 
-    def delete(self, uri, parameters=None):
+    def delete(self, uri: str, parameters: Optional[dict] = None) -> dict:
         """
 
         :param uri: Url from which user wants to delete the data
         :param parameters: These are query parameters
         :return: json response
         """
-        full_url = self.__baseurl + uri
+        full_url = self.__base_url + uri
 
         if parameters is not None:
             full_url = "%s?%s" % (full_url, urllib.parse.urlencode(parameters))
 
-        self.__headers["x-signature"] = sign(full_url, self.__eckey)
-        self.__headers["x-identity"] = get_compressed_public_key_from_pem(self.__eckey)
+        self.__headers["x-signature"] = sign(full_url, self.__ec_key)
+        self.__headers["x-identity"] = get_compressed_public_key_from_pem(self.__ec_key)
 
         response = requests.delete(full_url, headers=self.__headers)
         json_response = self.response_to_json_string(response)
         return json_response
 
-    def update(self, uri, form_data):
+    def update(self, uri: str, form_data: Any = {}) -> dict:
         """
         :param uri: Url from which user wants to delete the data
         :param form_data: the data to be updated
         :return: json response
         """
-        full_url = self.__baseurl + uri
+
+        full_url = self.__base_url + uri
         form_data = json.dumps(form_data)
 
-        self.__headers["x-signature"] = sign(full_url + form_data, self.__eckey)
-        self.__headers["x-identity"] = get_compressed_public_key_from_pem(self.__eckey)
+        self.__headers["x-signature"] = sign(full_url + form_data, self.__ec_key)
+        self.__headers["x-identity"] = get_compressed_public_key_from_pem(self.__ec_key)
 
         response = requests.put(full_url, data=form_data, headers=self.__headers)
         json_response = self.response_to_json_string(response)
         return json_response
 
-    def response_to_json_string(self, response):
+    def response_to_json_string(self, response: Response) -> Any:
         if not response.json():
             raise BitPayException("Error: HTTP response is null")
 
         response_obj = response.json()
         if "status" in response_obj:
             if response_obj["status"] == "error":
                 raise BitPayException(
                     "Error: " + response_obj["error"], response_obj["code"]
                 )
 
         if "error" in response_obj:
-            raise BitPayException(
-                "Error: " + response_obj["error"]
-            )
+            raise BitPayException("Error: " + response_obj["error"])
         elif "errors" in response_obj:
             message = ""
             for error in response_obj["errors"]:
                 message += "\n" + str(error)
             raise BitPayException("Errors: " + message)
 
         if "success" in response_obj:
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/Rate/rate.py` & `bitpay-4.0.0/src/bitpay/models/ledger/ledger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,58 @@
 """
-Rate
+Ledger
 """
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
 
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
-class Rate:
+
+class Ledger:
     """
-    Rate
+    Ledgers are records of money movement.
     """
 
-    __name = None
-    __code = None
-    __rate = None
+    __currency = None
+    __balance = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict):
         for key, value in kwargs.items():
             try:
+                value = ModelUtil.get_field_value(key, value, {"balance": "float"}, {})
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_name(self):
-        """
-        Get method for the name
-        :return: name
-        """
-        return self.__name
-
-    def set_name(self, name):
-        """
-        Set method for to name
-        :param name: name
-        """
-        self.__name = name
-
-    def get_code(self):
+    def get_currency(self) -> Optional[str]:
         """
-        Get method for the code
-        :return: code
+        Get method for to currency
+        :return: currency
         """
-        return self.__code
+        return self.__currency
 
-    def set_code(self, code):
+    def set_currency(self, currency: Optional[str]) -> None:
         """
-        Set method for to code
-        :param code: code
+        Set method for to currency
+        :param currency: currency
         """
-        self.__code = code
+        self.__currency = currency
 
-    def get_rate(self):
+    def get_balance(self) -> Optional[float]:
         """
-        Get method for the rate
-        :return: rate
+        Get method for to balance
+        :return: balance
         """
-        return self.__rate
+        return self.__balance
 
-    def set_rate(self, rate):
+    def set_balance(self, balance: Optional[float]) -> None:
         """
-        Set method for to rate
-        :param rate: rate
+        Set method for to balance
+        :param balance: balance
         """
-        self.__rate = rate
+        self.__balance = balance
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "name": self.get_name(),
-            "code": self.get_code(),
-            "rate": self.get_rate(),
-        }
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/Rate/rates.py` & `bitpay-4.0.0/src/bitpay/models/wallet/currency_qr.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,58 @@
 """
-Rates
+Currency Qr
 """
-from .rate import Rate
-from ..currency import Currency
-from ...exceptions.bitpay_exception import BitPayException
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
 
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
-class Rates:
+
+class CurrencyQr:
     """
-    Rates:Rates are exchange rates, representing the number of fiat
-    currency units equivalent to one BTC.
+    Currency Qr
     """
 
-    __bp = None
-    __rates = None
-
-    def __init__(self, rates, b_p, **kwargs):
-        self.set_bp(b_p)
-        self.set_rates(rates)
+    __type = None
+    __collapsed = None
 
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
+                value = ModelUtil.get_field_value(key, value, {"collapsed": "bool"}, {})
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_bp(self):
+    def get_type(self) -> Optional[str]:
         """
-        Get method for the bp
-        :return: bp
+        Get method for to type
+        :return: type
         """
-        return self.__bp
+        return self.__type
 
-    def set_bp(self, b_p):
+    def set_type(self, type: Optional[str]) -> None:
         """
-        Set method for the b_p
-        :param b_p: b_p
+        Set method for to type
+        :param type: type
         """
-        self.__bp = b_p
+        self.__type = type
 
-    def set_rates(self, rates):
+    def get_collapsed(self) -> Optional[bool]:
         """
-        Set method for the rates
-        :param rates: rates
+        Get method for to collapsed
+        :return: collapsed
         """
-        self.__rates = rates
-
-    def get_rates(self):
-        rates = []
-        for rate in self.__rates:
-            if isinstance(rate, Rate):
-                rates.append(rate.to_json())
-            else:
-                rates.append(rate)
-        return rates
-
-    def update(self):
-        self.__rates = self.__bp.get_rates().get_rates()
+        return self.__collapsed
 
-    def get_rate(self, currency_code):
-        if not Currency.is_valid(currency_code):
-            raise BitPayException("currency code must be a type of Model.Currency")
-
-        val = None
-        for rate_obj in self.__rates:
-            if rate_obj.get_code == currency_code:
-                val = rate_obj.get_rate()
-        return val
+    def set_collapsed(self, collapsed: Optional[bool]) -> None:
+        """
+        Set method for to collapsed
+        :param collapsed: collapsed
+        """
+        self.__collapsed = collapsed
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {"rates": self.get_rates()}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/ledger/buyer.py` & `bitpay-4.0.0/src/bitpay/models/ledger/buyer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,187 +1,177 @@
 """
 Buyer
 """
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
+
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class Buyer:
     """
     Allows merchant to pass buyer related information in the invoice object
     """
 
-    __name = ""
-    __address1 = ""
-    __address2 = ""
-    __city = ""
-    __state = ""
-    __zip = ""
-    __country = ""
-    __email = ""
-    __phone = ""
-    __notify = ""
+    __name = None
+    __address1 = None
+    __address2 = None
+    __city = None
+    __state = None
+    __zip = None
+    __country = None
+    __email = None
+    __phone = None
+    __notify = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_name(self):
+    def get_name(self) -> Optional[str]:
         """
         Get method for to name
         :return: name
         """
         return self.__name
 
-    def set_name(self, name):
+    def set_name(self, name: Optional[str]) -> None:
         """
         Set method for to name
         :param name: name
         """
         self.__name = name
 
-    def get_address1(self):
+    def get_address1(self) -> Optional[str]:
         """
         Get method for to address1
         :return: address1
         """
         return self.__address1
 
-    def set_address1(self, address1):
+    def set_address1(self, address1: Optional[str]) -> None:
         """
         Set method for to address1
         :param address1: address1
         """
         self.__address1 = address1
 
-    def get_address2(self):
+    def get_address2(self) -> Optional[str]:
         """
         Get method for to address2
         :return: address2
         """
         return self.__address2
 
-    def set_address2(self, address2):
+    def set_address2(self, address2: Optional[str]) -> None:
         """
         Set method for to address2
         :param address2: address2
         """
         self.__address2 = address2
 
-    def get_city(self):
+    def get_city(self) -> Optional[str]:
         """
         Get method for to city
         :return: city
         """
         return self.__city
 
-    def set_city(self, city):
+    def set_city(self, city: Optional[str]) -> None:
         """
         Set method for to city
         :param city: city
         """
         self.__city = city
 
-    def get_state(self):
+    def get_state(self) -> Optional[str]:
         """
         Get method for to state
         :return: state
         """
         return self.__state
 
-    def set_state(self, state):
+    def set_state(self, state: Optional[str]) -> None:
         """
         Set method for to state
         :param state: state
         """
         self.__state = state
 
-    def get_zip(self):
+    def get_zip(self) -> Optional[str]:
         """
         Get method for to zip
         :return: zip
         """
         return self.__zip
 
-    def set_zip(self, zip):
+    def set_zip(self, zip: Optional[str]) -> None:
         """
         Set method for to zip
         :param zip: zip
         """
         self.__zip = zip
 
-    def get_country(self):
+    def get_country(self) -> Optional[str]:
         """
         Get method for to country
         :return: country
         """
         return self.__country
 
-    def set_country(self, country):
+    def set_country(self, country: Optional[str]) -> None:
         """
         Set method for to country
         :param country: country
         """
         self.__country = country
 
-    def get_email(self):
+    def get_email(self) -> Optional[str]:
         """
         Get method for to email
         :return: email
         """
         return self.__email
 
-    def set_email(self, email):
+    def set_email(self, email: Optional[str]) -> None:
         """
         Set method for to email
         :param email: email
         """
         self.__email = email
 
-    def get_phone(self):
+    def get_phone(self) -> Optional[str]:
         """
         Get method for to phone
         :return: phone
         """
         return self.__phone
 
-    def set_phone(self, phone):
+    def set_phone(self, phone: Optional[str]) -> None:
         """
         Set method for to phone
         :param phone: phone
         """
         self.__phone = phone
 
-    def get_notify(self):
+    def get_notify(self) -> Optional[str]:
         """
         Get method for to notify
         :return: notify
         """
         return self.__notify
 
-    def set_notify(self, notify):
+    def set_notify(self, notify: Optional[str]) -> None:
         """
         Set method for to notify
         :param notify: notify
         """
         self.__notify = notify
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "name": self.get_name(),
-            "address1": self.get_address1(),
-            "address2": self.get_address2(),
-            "city": self.get_city(),
-            "state": self.get_state(),
-            "zip": self.get_zip(),
-            "country": self.get_country(),
-            "email": self.get_email(),
-            "phone": self.get_phone(),
-            "notify": self.get_notify(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/ledger/ledger_entry.py` & `bitpay-4.0.0/src/bitpay/models/ledger/ledger_entry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
 LedgerEntry
 """
-from ...models.ledger.buyer import Buyer
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
+
+from bitpay.models.ledger.buyer import Buyer
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class LedgerEntry:
     """
     Ledger entry
     """
 
@@ -25,260 +28,235 @@
     # Buyer
     __buyer_fields = Buyer()
 
     __invoice_amount = None
     __invoice_currency = None
     __transaction_currency = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
-                if key in ["buyerFields"]:
-                    klass = (
-                        Buyer
-                        if key == "buyerFields"
-                        else globals()[key[0].upper() + key[1:]]
-                    )
-                    if isinstance(value, list):
-                        objs = []
-                        for obj in value:
-                            objs.append(klass(**obj))
-                        value = objs
-                    else:
-                        value = klass(**value)
+                value = ModelUtil.get_field_value(
+                    key,
+                    value,
+                    {"amount": "float", "invoiceAmount": "float", "buyerFields": Buyer},
+                    {},
+                )
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_type(self):
+    def get_type(self) -> Optional[str]:
         """
         Get method for to type
         :return: type
         """
         return self.__type
 
-    def set_type(self, type):
+    def set_type(self, type: Optional[str]) -> None:
         """
         Set method for to type
         :param type: type
         """
         self.__type = type
 
-    def get_amount(self):
+    def get_amount(self) -> Optional[float]:
         """
         Get method for to amount
         :return: amount
         """
         return self.__amount
 
-    def set_amount(self, amount):
+    def set_amount(self, amount: Optional[float]) -> None:
         """
         Set method for to amount
         :param amount: amount
         """
         self.__amount = amount
 
-    def get_code(self):
+    def get_code(self) -> Optional[str]:
         """
         Get method for to code
         :return: code
         """
         return self.__code
 
-    def set_code(self, code):
+    def set_code(self, code: Optional[str]) -> None:
         """
         Set method for to code
         :param code: code
         """
         self.__code = code
 
-    def get_timestamp(self):
+    def get_timestamp(self) -> Optional[str]:
         """
         Get method for to timestamp
         :return: timestamp
         """
         return self.__timestamp
 
-    def set_timestamp(self, timestamp):
+    def set_timestamp(self, timestamp: Optional[str]) -> None:
         """
         Set method for to timestamp
         :param timestamp: timestamp
         """
         self.__timestamp = timestamp
 
-    def get_currency(self):
+    def get_currency(self) -> Optional[str]:
         """
         Get method for to currency
         :return: currency
         """
         return self.__currency
 
-    def set_currency(self, currency):
+    def set_currency(self, currency: Optional[str]) -> None:
         """
         Set method for to currency
         :param currency: currency
         """
         self.__currency = currency
 
-    def get_tx_type(self):
+    def get_tx_type(self) -> Optional[str]:
         """
         Get method for to tx_type
         :return: tx_type
         """
         return self.__tx_type
 
-    def set_tx_type(self, tx_type):
+    def set_tx_type(self, tx_type: Optional[str]) -> None:
         """
         Set method for to tx_type
         :param tx_type: tx_type
         """
         self.__tx_type = tx_type
 
-    def get_scale(self):
+    def get_scale(self) -> Optional[str]:
         """
         Get method for to scale
         :return: scale
         """
         return self.__scale
 
-    def set_scale(self, scale):
+    def set_scale(self, scale: Optional[str]) -> None:
         """
         Set method for to scale
         :param scale: scale
         """
         self.__scale = scale
 
-    def get_id(self):
+    def get_id(self) -> Optional[str]:
         """
         Get method for to id
         :return: id
         """
         return self.__id
 
-    def set_id(self, id):
+    def set_id(self, id: Optional[str]) -> None:
         """
         Set method for to id
         :param id: id
         """
         self.__id = id
 
-    def get_support_request(self):
+    def get_support_request(self) -> Optional[str]:
         """
         Get method for to support_request
         :return: support_request
         """
         return self.__support_request
 
-    def set_support_request(self, support_request):
+    def set_support_request(self, support_request: Optional[str]) -> None:
         """
         Set method for to support_request
         :param support_request: support_request
         """
         self.__support_request = support_request
 
-    def get_description(self):
+    def get_description(self) -> Optional[str]:
         """
         Get method for to description
         :return: description
         """
         return self.__description
 
-    def set_description(self, description):
+    def set_description(self, description: Optional[str]) -> None:
         """
         Set method for to description
         :param description: description
         """
         self.__description = description
 
-    def get_invoice_id(self):
+    def get_invoice_id(self) -> Optional[str]:
         """
         Get method for to invoice_id
         :return: invoice_id
         """
         return self.__invoice_id
 
-    def set_invoice_id(self, invoice_id):
+    def set_invoice_id(self, invoice_id: Optional[str]) -> None:
         """
         Set method for to invoice_id
         :param invoice_id: invoice_id
         """
         self.__invoice_id = invoice_id
 
-    def get_buyer_fields(self):
+    def get_buyer_fields(self) -> Optional[Buyer]:
         """
         Get method for to buyer_fields
         :return: buyer_fields
         """
         return self.__buyer_fields
 
-    def set_buyer_fields(self, buyer_fields: Buyer):
+    def set_buyer_fields(self, buyer_fields: Buyer) -> None:
         """
         Set method for to buyer_fields
         :param buyer_fields: buyer_fields
         """
         self.__buyer_fields = buyer_fields
 
-    def get_invoice_amount(self):
+    def get_invoice_amount(self) -> Optional[float]:
         """
         Get method for to invoice_amount
         :return: invoice_amount
         """
         return self.__invoice_amount
 
-    def set_invoice_amount(self, invoice_amount):
+    def set_invoice_amount(self, invoice_amount: Optional[float]) -> None:
         """
         Set method for to invoice_amount
         :param invoice_amount: invoice_amount
         """
         self.__invoice_amount = invoice_amount
 
-    def get_invoice_currency(self):
+    def get_invoice_currency(self) -> Optional[str]:
         """
         Get method for to invoice_currency
         :return: invoice_currency
         """
         return self.__invoice_currency
 
-    def set_invoice_currency(self, invoice_currency):
+    def set_invoice_currency(self, invoice_currency: Optional[str]) -> None:
         """
         Set method for to invoice_currency
         :param invoice_currency: invoice_currency
         """
         self.__invoice_currency = invoice_currency
 
-    def get_transaction_currency(self):
+    def get_transaction_currency(self) -> Optional[str]:
         """
         Get method for to transaction_currency
         :return: transaction_currency
         """
         return self.__transaction_currency
 
-    def set_transaction_currency(self, transaction_currency):
+    def set_transaction_currency(self, transaction_currency: Optional[str]) -> None:
         """
         Set method for to transaction_currency
         :param transaction_currency: transaction_currency
         """
         self.__transaction_currency = transaction_currency
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "type": self.get_type(),
-            "amount": self.get_amount(),
-            "code": self.get_code(),
-            "timestamp": self.get_timestamp(),
-            "currency": self.get_currency(),
-            "txType": self.get_tx_type(),
-            "scale": self.get_scale(),
-            "id": self.get_id(),
-            "supportRequest": self.get_support_request(),
-            "description": self.get_description(),
-            "invoiceId": self.get_invoice_id(),
-            "buyerFields": self.get_buyer_fields().to_json(),
-            "invoiceAmount": self.get_invoice_amount(),
-            "invoiceCurrency": self.get_invoice_currency(),
-            "transactionCurrency": self.get_transaction_currency(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/bill/bill.py` & `bitpay-4.0.0/src/bitpay/models/bill/bill.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,421 +1,376 @@
 """
 Bill
 """
+from typing import List, Optional
+
 from .item import Item
-from ..currency import Currency
-from ...exceptions.bitpay_exception import BitPayException
-from ...utils.key_utils import change_camel_case_to_snake_case
+from bitpay.models.currency import Currency
+from bitpay.exceptions.bitpay_exception import BitPayException
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class Bill:
     """
     Bills are payment requests addressed to specific buyers.
     Bill line items have fixed prices, typically denominated
     in fiat currency.
     """
 
     __currency = None
-    __token = ""
+    __token = None
     __email = None
-    __items = None
+    __items: Optional[List[Item]] = None
     __number = None
     __name = None
     __address1 = None
     __address2 = None
     __city = None
     __state = None
     __zip = None
     __country = None
-    __cc = None
-    __delivered = None
+    __cc: Optional[List[str]] = None
     __phone = None
     __due_date = None
-    __pass_processing_fee = None
+    __pass_processing_fee = False
     __status = None
     __url = None
     __created_date = None
     __email_bill = None
     __id = None
     __merchant = None
 
-    def __init__(self, number=None, currency=None, email=None, **kwargs):
+    def __init__(
+        self,
+        number: Optional[str] = None,
+        currency: Optional[str] = None,
+        email: Optional[str] = None,
+        **kwargs: dict
+    ) -> None:
         self.set_number(number)
-        self.set_currency(currency)
         self.set_email(email)
+        if currency is not None:
+            self.set_currency(currency)
 
         for key, value in kwargs.items():
             try:
-                if key in ["items"]:
-                    klass = (
-                        Item if key == "items" else globals()[key[0].upper() + key[1:]]
-                    )
-
-                    if isinstance(value, list):
-                        objs = []
-                        for obj in value:
-                            objs.append(klass(**obj))
-                        value = objs
-                    else:
-                        value = klass(**value)
+                value = ModelUtil.get_field_value(key, value, {}, {"items": Item})
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_currency(self):
+    def get_currency(self) -> Optional[str]:
         """
         Get method for to currency
         :return: currency
         """
         return self.__currency
 
-    def set_currency(self, currency):
+    def set_currency(self, currency: str) -> None:
         """
         Set method for to currency
         :param currency: currency
         """
         if not Currency.is_valid(currency):
             raise BitPayException("currency code must be a type of Model.Currency")
         self.__currency = currency
 
-    def get_token(self):
+    def get_token(self) -> Optional[str]:
         """
         Get method for to token
         :return: token
         """
         return self.__token
 
-    def set_token(self, token):
+    def set_token(self, token: Optional[str]) -> None:
         """
         Set method for to token
         :param token: token
         """
         self.__token = token
 
-    def get_delivered(self):
-        """
-        Get method for to delivered
-        :return: delivered
-        """
-        return self.__delivered
-
-    def set_delivered(self, delivered):
-        """
-        Set method for to delivered
-        :param delivered: delivered
-        """
-        self.__delivered = delivered
-
-    def get_email(self):
+    def get_email(self) -> Optional[str]:
         """
         Get method for to email
         :return: email
         """
         return self.__email
 
-    def set_email(self, email):
+    def set_email(self, email: Optional[str]) -> None:
         """
         Set method for to email
         :param email: email
         """
         self.__email = email
 
-    def get_number(self):
+    def get_number(self) -> Optional[str]:
         """
         Get method for to number
         :return: number
         """
         return self.__number
 
-    def set_number(self, number):
+    def set_number(self, number: Optional[str]) -> None:
         """
         Set method for to number
         :param number: number
         """
         self.__number = number
 
-    def get_name(self):
+    def get_name(self) -> Optional[str]:
         """
         Get method for to name
         :return: name
         """
         return self.__name
 
-    def set_name(self, name):
+    def set_name(self, name: Optional[str]) -> None:
         """
         Set method for to name
         :param name: name
         """
         self.__name = name
 
-    def get_address1(self):
+    def get_address1(self) -> Optional[str]:
         """
         Get method for to address1
         :return: address1
         """
         return self.__address1
 
-    def set_address1(self, address1):
+    def set_address1(self, address1: Optional[str]) -> None:
         """
         Set method for to address1
         :param address1: address1
         """
         self.__address1 = address1
 
-    def get_address2(self):
+    def get_address2(self) -> Optional[str]:
         """
         Get method for to address2
         :return: address2
         """
         return self.__address2
 
-    def set_address2(self, address2):
+    def set_address2(self, address2: Optional[str]) -> None:
         """
         Set method for to address2
         :param address2: address2
         """
         self.__address2 = address2
 
-    def get_city(self):
+    def get_city(self) -> Optional[str]:
         """
         Get method for to city
         :return: city
         """
         return self.__city
 
-    def set_city(self, city):
+    def set_city(self, city: Optional[str]) -> None:
         """
         Set method for to city
         :param city: city
         """
         self.__city = city
 
-    def get_state(self):
+    def get_state(self) -> Optional[str]:
         """
         Get method for to state
         :return: state
         """
         return self.__state
 
-    def set_state(self, state):
+    def set_state(self, state: Optional[str]) -> None:
         """
         Set method for to state
         :param state: state
         """
         self.__state = state
 
-    def get_zip(self):
+    def get_zip(self) -> Optional[str]:
         """
         Get method for to zip
         :return: zip
         """
         return self.__zip
 
-    def set_zip(self, zip):
+    def set_zip(self, zip: Optional[str]) -> None:
         """
         Set method for to zip
         :param zip: zip
         """
         self.__zip = zip
 
-    def get_country(self):
+    def get_country(self) -> Optional[str]:
         """
         Get method for to country
         :return: country
         """
         return self.__country
 
-    def set_country(self, country):
+    def set_country(self, country: Optional[str]) -> None:
         """
         Set method for to country
         :param country: country
         """
         self.__country = country
 
-    def get_cc(self):
+    def get_cc(self) -> Optional[List[str]]:
         """
         Get method for to cc
         :return: cc
         """
         return self.__cc
 
-    def set_cc(self, cc):
+    def set_cc(self, cc: Optional[List[str]]) -> None:
         """
         Set method for to cc
         :param cc: cc
         """
         self.__cc = cc
 
-    def get_phone(self):
+    def get_phone(self) -> Optional[str]:
         """
         Get method for to phone
         :return: phone
         """
         return self.__phone
 
-    def set_phone(self, phone):
+    def set_phone(self, phone: Optional[str]) -> None:
         """
         Set method for to phone
         :param phone: phone
         """
         self.__phone = phone
 
-    def get_due_date(self):
+    def get_due_date(self) -> Optional[str]:
         """
         Get method for to due_date
         :return: due_date
         """
         return self.__due_date
 
-    def set_due_date(self, due_date):
+    def set_due_date(self, due_date: Optional[str]) -> None:
         """
         Set method for to due_date
         :param due_date: due_date
         """
         self.__due_date = due_date
 
-    def get_pass_processing_fee(self):
+    def get_pass_processing_fee(self) -> bool:
         """
         Get method for to pass_processing_fee
         :return: pass_processing_fee
         """
         return self.__pass_processing_fee
 
-    def set_pass_processing_fee(self, pass_processing_fee):
+    def set_pass_processing_fee(self, pass_processing_fee: bool) -> None:
         """
         Set method for to pass_processing_fee
         :param pass_processing_fee: pass_processing_fee
         """
         self.__pass_processing_fee = pass_processing_fee
 
-    def get_status(self):
+    def get_status(self) -> Optional[str]:
         """
         Get method for to status
         :return: status
         """
         return self.__status
 
-    def set_status(self, status):
+    def set_status(self, status: Optional[str]) -> None:
         """
         Set method for to status
         :param status: status
         """
         self.__status = status
 
-    def get_url(self):
+    def get_url(self) -> Optional[str]:
         """
         Get method for to url
         :return: url
         """
         return self.__url
 
-    def set_url(self, url):
+    def set_url(self, url: Optional[str]) -> None:
         """
         Set method for to url
         :param url: url
         """
         self.__url = url
 
-    def get_created_date(self):
+    def get_created_date(self) -> Optional[str]:
         """
         Get method for to created_date
         :return: created_date
         """
         return self.__created_date
 
-    def set_created_date(self, created_date):
+    def set_created_date(self, created_date: Optional[str]) -> None:
         """
         Set method for to created_date
         :param created_date: created_date
         """
         self.__created_date = created_date
 
-    def get_email_bill(self):
+    def get_email_bill(self) -> Optional[str]:
         """
         Get method for to email_bill
         :return: email_bill
         """
         return self.__email_bill
 
-    def set_email_bill(self, email_bill):
+    def set_email_bill(self, email_bill: Optional[str]) -> None:
         """
         Set method for to email_bill
         :param email_bill: email_bill
         """
         self.__email_bill = email_bill
 
-    def get_id(self):
+    def get_id(self) -> Optional[str]:
         """
         Get method for to id
         :return: id
         """
         return self.__id
 
-    def set_id(self, id):
+    def set_id(self, value: Optional[str]) -> None:
         """
         Set method for to id
-        :param id: id
+        :param value: id
         """
-        self.__id = id
+        self.__id = value
 
-    def get_merchant(self):
+    def get_merchant(self) -> Optional[str]:
         """
         Get method for to merchant
         :return: merchant
         """
         return self.__merchant
 
-    def set_merchant(self, merchant):
+    def set_merchant(self, merchant: Optional[str]) -> None:
         """
         Set method for to merchant
         :param merchant: merchant
         """
         self.__merchant = merchant
 
-    def get_items(self):
+    def get_items(self) -> Optional[List[Item]]:
         """
         Get method for to item
         :return: item
         """
         return self.__items
 
-    def set_items(self, item: [Item]):
+    def set_items(self, item: Optional[List[Item]]) -> None:
         """
         Set method for to item
         :param item: item
         """
         self.__items = item
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        items = []
-        for item in self.get_items():
-            items.append(item.to_json())
-        data = {
-            "currency": self.get_currency(),
-            "token": self.get_token(),
-            "email": self.get_email(),
-            "items": items,
-            "number": self.get_number(),
-            "name": self.get_name(),
-            "address1": self.get_address1(),
-            "address2": self.get_address2(),
-            "city": self.get_city(),
-            "state": self.get_state(),
-            "zip": self.get_zip(),
-            "country": self.get_country(),
-            "cc": self.get_cc(),
-            "phone": self.get_phone(),
-            "dueDate": self.get_due_date(),
-            "passProcessingFee": self.get_pass_processing_fee(),
-            "status": self.get_status(),
-            "url": self.get_url(),
-            "createdDate": self.get_created_date(),
-            "delivered": self.get_delivered(),
-            "emailBill": self.get_email_bill(),
-            "id": self.get_id(),
-            "merchant": self.get_merchant(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/settlement/settlement_ledger_entry.py` & `bitpay-4.0.0/src/bitpay/models/settlement/settlement_ledger_entry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,145 +1,144 @@
 """
 SettlementLedgerEntry: ledger entries in the settlement,
 """
+from typing import Optional
+
 from .invoice_data import InvoiceData
-from ...utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class SettlementLedgerEntry:
     """
     SettlementLedgerEntry
     """
 
     __code = None
     __invoice_id = None
     __amount = None
     __timestamp = None
     __description = None
     __reference = None
-    __invoice_data = InvoiceData()
+    __invoice_data: Optional[InvoiceData] = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
-                if key in [
-                    "invoiceData",
-                ]:
-                    klass = globals()[key[0].upper() + key[1:]]
-                    value = klass(**value)
+                value = ModelUtil.get_field_value(
+                    key,
+                    value,
+                    {
+                        "invoiceData": InvoiceData,
+                        "code": "int",
+                        "amount": "float",
+                        "timestamp": "str",
+                    },
+                    {},
+                )
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_code(self):
+    def get_code(self) -> Optional[int]:
         """
         Get method for the code
         :return: code
         """
         return self.__code
 
-    def set_code(self, code):
+    def set_code(self, code: Optional[int]) -> None:
         """
         Set method for the code
         :param code: code
         """
         self.__code = code
 
-    def get_invoice_id(self):
+    def get_invoice_id(self) -> Optional[str]:
         """
         Get method for the invoice_id
         :return: invoice_id
         """
         return self.__invoice_id
 
-    def set_invoice_id(self, invoice_id):
+    def set_invoice_id(self, invoice_id: Optional[str]) -> None:
         """
         Set method for the invoice_id
         :param invoice_id: invoice_id
         """
         self.__invoice_id = invoice_id
 
-    def get_amount(self):
+    def get_amount(self) -> Optional[float]:
         """
         Get method for the amount
         :return: amount
         """
         return self.__amount
 
-    def set_amount(self, amount):
+    def set_amount(self, amount: Optional[float]) -> None:
         """
         Set method for the amount
         :param amount: amount
         """
         self.__amount = amount
 
-    def get_timestamp(self):
+    def get_timestamp(self) -> Optional[str]:
         """
         Get method for the timestamp
         :return: timestamp
         """
         return self.__timestamp
 
-    def set_timestamp(self, timestamp):
+    def set_timestamp(self, timestamp: Optional[str]) -> None:
         """
         Set method for the timestamp
         :param timestamp: timestamp
         """
         self.__timestamp = timestamp
 
-    def get_description(self):
+    def get_description(self) -> Optional[str]:
         """
         Get method for the description
         :return: description
         """
         return self.__description
 
-    def set_description(self, description):
+    def set_description(self, description: Optional[str]) -> None:
         """
         Set method for the description
         :param description: description
         """
         self.__description = description
 
-    def get_reference(self):
+    def get_reference(self) -> Optional[str]:
         """
         Get method for the reference
         :return: reference
         """
         return self.__reference
 
-    def set_reference(self, reference):
+    def set_reference(self, reference: Optional[str]) -> None:
         """
         Set method for the reference
         :param reference: reference
         """
         self.__reference = reference
 
-    def get_invoice_data(self):
+    def get_invoice_data(self) -> Optional[InvoiceData]:
         """
         Get method for the invoice_data
         :return: invoice_data
         """
         return self.__invoice_data
 
-    def set_invoice_data(self, invoice_data: InvoiceData):
+    def set_invoice_data(self, invoice_data: Optional[InvoiceData]) -> None:
         """
         Set method for the invoice_data
         :param invoice_data: invoice_data
         """
         self.__invoice_data = invoice_data
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "code": self.get_code(),
-            "invoiceId": self.get_invoice_id(),
-            "amount": self.get_amount(),
-            "timestamp": self.get_timestamp(),
-            "description": self.get_description(),
-            "reference": self.get_reference(),
-            "invoiceData": self.get_invoice_data().to_json(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/settlement/invoice_data.py` & `bitpay-4.0.0/src/bitpay/models/settlement/invoice_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
 InvoiceData: Object containing relevant information from the paid invoice
 """
-from ...models.settlement.refund_info import RefundInfo
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional, List
+
+from bitpay.models.settlement.refund_info import RefundInfo
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class InvoiceData:
     """
     invoice data
     """
 
@@ -14,187 +17,161 @@
     __date = None
     __price = None
     __currency = None
     __transaction_currency = None
     __over_paid_amount = None
     __payout_percentage = None
     __buyer_email_address = None
-    __btc_price = None
     """
     RefundInfo
     """
     __refund_info = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
-                if key in ["refundInfo"]:
-                    klass = globals()[key[0].upper() + key[1:]]
-
-                    if isinstance(value, list):
-                        objs = []
-                        for obj in value:
-                            objs.append(klass(**obj))
-                        value = objs
-                    else:
-                        value = klass(**value)
+                value = ModelUtil.get_field_value(
+                    key,
+                    value,
+                    {
+                        "refundInfo": RefundInfo,
+                        "date": "str",
+                        "price": "float",
+                        "overPaidAmount": "float",
+                    },
+                    {"payoutPercentage": "dict"},
+                )
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_order_id(self):
+    def get_order_id(self) -> Optional[str]:
         """
         Get method for to order_id
         :return: order_id
         """
         return self.__order_id
 
-    def set_order_id(self, order_id):
+    def set_order_id(self, order_id: Optional[str]) -> None:
         """
         Set method for to order_id
         :param order_id: order_id
         """
         self.__order_id = order_id
 
-    def get_buyer_email_address(self):
+    def get_buyer_email_address(self) -> Optional[str]:
         """
         Get method for to buyer_email_address
         :return: buyer_email_address
         """
         return self.__buyer_email_address
 
-    def set_buyer_email_address(self, buyer_email_address):
+    def set_buyer_email_address(self, buyer_email_address: Optional[str]) -> None:
         """
         Set method for to buyer_email_address
         :param buyer_email_address: buyer_email_address
         """
         self.__buyer_email_address = buyer_email_address
 
-    def get_date(self):
+    def get_date(self) -> Optional[str]:
         """
         Get method for to date
         :return: date
         """
         return self.__date
 
-    def set_date(self, date):
+    def set_date(self, date: Optional[str]) -> None:
         """
         Set method for to date
         :param date: date
         """
         self.__date = date
 
-    def get_price(self):
+    def get_price(self) -> Optional[float]:
         """
         Get method for to price
         :return: price
         """
         return self.__price
 
-    def set_price(self, price):
+    def set_price(self, price: Optional[float]) -> None:
         """
         Set method for to price
         :param price: price
         """
         self.__price = price
 
-    def get_currency(self):
+    def get_currency(self) -> Optional[str]:
         """
         Get method for to currency
         :return: currency
         """
         return self.__currency
 
-    def set_currency(self, currency):
+    def set_currency(self, currency: Optional[str]) -> None:
         """
         Set method for to currency
         :param currency: currency
         """
         self.__currency = currency
 
-    def get_transaction_currency(self):
+    def get_transaction_currency(self) -> Optional[str]:
         """
         Get method for to transaction_currency
         :return: transaction_currency
         """
         return self.__transaction_currency
 
-    def set_transaction_currency(self, transaction_currency):
+    def set_transaction_currency(self, transaction_currency: Optional[str]) -> None:
         """
         Set method for to transaction_currency
         :param transaction_currency: transaction_currency
         """
         self.__transaction_currency = transaction_currency
 
-    def get_over_paid_amount(self):
+    def get_over_paid_amount(self) -> Optional[float]:
         """
         Get method for to over_paid_amount
         :return: over_paid_amount
         """
         return self.__over_paid_amount
 
-    def set_over_paid_amount(self, over_paid_amount):
+    def set_over_paid_amount(self, over_paid_amount: Optional[float]) -> None:
         """
         Set method for to over_paid_amount
         :param over_paid_amount: over_paid_amount
         """
         self.__over_paid_amount = over_paid_amount
 
-    def get_payout_percentage(self):
+    def get_payout_percentage(self) -> Optional[List[dict]]:
         """
         Get method for to payout_percentage
         :return: payout_percentage
         """
         return self.__payout_percentage
 
-    def set_payout_percentage(self, payout_percentage):
+    def set_payout_percentage(self, payout_percentage: Optional[List[dict]]) -> None:
         """
         Set method for to payout_percentage
         :param payout_percentage: transaction_currency
         """
         self.__payout_percentage = payout_percentage
 
-    def get_btc_price(self):
-        """
-        Get method for to btc_price
-        :return: btc_price
-        """
-        return self.__btc_price
-
-    def set_btc_price(self, btc_price):
-        """
-        Set method for to btc_price
-        :param btc_price: btc_price
-        """
-        self.__btc_price = btc_price
-
-    def get_refund_info(self):
+    def get_refund_info(self) -> Optional[RefundInfo]:
         """
         Get method for to refund_info
         :return: refund_info
         """
         return self.__refund_info
 
-    def set_refund_info(self, refund_info: RefundInfo):
+    def set_refund_info(self, refund_info: Optional[RefundInfo]) -> None:
         """
         Set method for to refund_info
         :param refund_info: refund_info
         """
         self.__refund_info = refund_info
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "orderId": self.get_order_id(),
-            "date": self.get_date(),
-            "price": self.get_price(),
-            "currency": self.get_currency(),
-            "transactionCurrency": self.get_transaction_currency(),
-            "buyerEmailAddress": self.get_buyer_email_address(),
-            "payoutPercentage": self.get_payout_percentage(),
-            "refundInfo": self.get_refund_info().to_json(),
-            "btcPrice": self.get_btc_price(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/settlement/payout_info.py` & `bitpay-4.0.0/src/bitpay/models/settlement/payout_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
 PayoutInfo: Object containing the settlement info provided by the Merchant
 in his BitPay account settings
 """
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
+
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class PayoutInfo:
     """
     PayoutInfo
     """
 
@@ -31,383 +34,364 @@
     __account_holder_name = None
     __account_holder_address = None
     __account_holder_address2 = None
     __account_holder_postal_code = None
     __account_holder_city = None
     __account_holder_country = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
                 if key == "merchantEIN":
-                    self.set_merchant_ein(value)
+                    self.set_merchant_ein(str(value))
                 else:
                     getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(
                         value
                     )
             except AttributeError:
                 pass
 
-    def get_name(self):
+    def get_name(self) -> Optional[str]:
         """
         Get method for to name
         :return: name
         """
         return self.__name
 
-    def set_name(self, name):
+    def set_name(self, name: Optional[str]) -> None:
         """
         Set method for to name
         :param name: name
         """
         self.__name = name
 
-    def get_account(self):
+    def get_account(self) -> Optional[str]:
         """
         Get method for to account
         :return: account
         """
         return self.__account
 
-    def set_account(self, account):
+    def set_account(self, account: Optional[str]) -> None:
         """
         Set method for to account
         :param account: account
         """
         self.__account = account
 
-    def get_routing(self):
+    def get_routing(self) -> Optional[str]:
         """
         Get method for to routing
         :return: routing
         """
         return self.__routing
 
-    def set_routing(self, routing):
+    def set_routing(self, routing: Optional[str]) -> None:
         """
         Set method for to routing
         :param routing: routing
         """
         self.__routing = routing
 
-    def get_merchant_ein(self):
+    def get_merchant_ein(self) -> Optional[str]:
         """
         Get method for to merchant_ein
         :return: merchant_ein
         """
         return self.__merchant_ein
 
-    def set_merchant_ein(self, merchant_ein):
+    def set_merchant_ein(self, merchant_ein: Optional[str]) -> None:
         """
         Set method for to merchant_ein
         :param merchant_ein: merchant_ein
         """
         self.__merchant_ein = merchant_ein
 
-    def get_label(self):
+    def get_label(self) -> Optional[str]:
         """
         Get method for to label
         :return: label
         """
         return self.__label
 
-    def set_label(self, label):
+    def set_label(self, label: Optional[str]) -> None:
         """
         Set method for to label
         :param label: label
         """
         self.__label = label
 
-    def get_bank_country(self):
+    def get_bank_country(self) -> Optional[str]:
         """
         Get method for to bank_country
         :return: bank_country
         """
         return self.__bank_country
 
-    def set_bank_country(self, bank_country):
+    def set_bank_country(self, bank_country: Optional[str]) -> None:
         """
         Set method for to bank_country
         :param bank_country: bank_country
         """
         self.__bank_country = bank_country
 
-    def get_bank(self):
+    def get_bank(self) -> Optional[str]:
         """
         Get method for to bank
         :return: bank
         """
         return self.__bank
 
-    def set_bank(self, bank):
+    def set_bank(self, bank: Optional[str]) -> None:
         """
         Set method for to bank
         :param bank: bank
         """
         self.__bank = bank
 
-    def get_swift(self):
+    def get_swift(self) -> Optional[str]:
         """
         Get method for to swift
         :return: swift
         """
         return self.__swift
 
-    def set_swift(self, swift):
+    def set_swift(self, swift: Optional[str]) -> None:
         """
         Set method for to swift
         :param swift: swift
         """
         self.__swift = swift
 
-    def get_address(self):
+    def get_address(self) -> Optional[str]:
         """
         Get method for to address
         :return: address
         """
         return self.__address
 
-    def set_address(self, address):
+    def set_address(self, address: Optional[str]) -> None:
         """
         Set method for to address
         :param address: address
         """
         self.__address = address
 
-    def get_city(self):
+    def get_city(self) -> Optional[str]:
         """
         Get method for to city
         :return: city
         """
         return self.__city
 
-    def set_city(self, city):
+    def set_city(self, city: Optional[str]) -> None:
         """
         Set method for to city
         :param city: city
         """
         self.__city = city
 
-    def get_postal(self):
+    def get_postal(self) -> Optional[str]:
         """
         Get method for to postal
         :return: postal
         """
         return self.__postal
 
-    def set_postal(self, postal):
+    def set_postal(self, postal: Optional[str]) -> None:
         """
         Set method for to postal
         :param postal: postal
         """
         self.__postal = postal
 
-    def get_sort(self):
+    def get_sort(self) -> Optional[str]:
         """
         Get method for to sort
         :return: sort
         """
         return self.__sort
 
-    def set_sort(self, sort):
+    def set_sort(self, sort: Optional[str]) -> None:
         """
         Set method for to sort
         :param sort: sort
         """
         self.__sort = sort
 
-    def get_wire(self):
+    def get_wire(self) -> Optional[str]:
         """
         Get method for to wire
         :return: wire
         """
         return self.__wire
 
-    def set_wire(self, wire):
+    def set_wire(self, wire: Optional[str]) -> None:
         """
         Set method for to wire
         :param wire: wire
         """
         self.__wire = wire
 
-    def get_bank_name(self):
+    def get_bank_name(self) -> Optional[str]:
         """
         Get method for to bank_name
         :return: bank_name
         """
         return self.__bank_name
 
-    def set_bank_name(self, bank_name):
+    def set_bank_name(self, bank_name: Optional[str]) -> None:
         """
         Set method for to bank_name
         :param bank_name: bank_name
         """
         self.__bank_name = bank_name
 
-    def get_bank_address(self):
+    def get_bank_address(self) -> Optional[str]:
         """
         Get method for to bank_address
         :return: bank_address
         """
         return self.__bank_address
 
-    def set_bank_address(self, bank_address):
+    def set_bank_address(self, bank_address: Optional[str]) -> None:
         """
         Set method for to bank_address
         :param bank_address: bank_address
         """
         self.__bank_address = bank_address
 
-    def get_bank_address2(self):
+    def get_bank_address2(self) -> Optional[str]:
         """
         Get method for to bank_address2
         :return: bank_address2
         """
         return self.__bank_address2
 
-    def set_bank_address2(self, bank_address2):
+    def set_bank_address2(self, bank_address2: Optional[str]) -> None:
         """
         Set method for to bank_address2
         :param bank_address2: bank_address2
         """
         self.__bank_address2 = bank_address2
 
-    def get_iban(self):
+    def get_iban(self) -> Optional[str]:
         """
         Get method for to iban
         :return: iban
         """
         return self.__iban
 
-    def set_iban(self, iban):
+    def set_iban(self, iban: Optional[str]) -> None:
         """
         Set method for to iban
         :param iban: iban
         """
         self.__iban = iban
 
-    def get_additional_information(self):
+    def get_additional_information(self) -> Optional[str]:
         """
         Get method for to additional_information
         :return: additional_information
         """
         return self.__additional_information
 
-    def set_additional_information(self, additional_information):
+    def set_additional_information(self, additional_information: Optional[str]) -> None:
         """
         Set method for to additional_information
         :param additional_information: additional_information
         """
         self.__additional_information = additional_information
 
-    def get_account_holder_name(self):
+    def get_account_holder_name(self) -> Optional[str]:
         """
         Get method for to account_holder_name
         :return: account_holder_name
         """
         return self.__account_holder_name
 
-    def set_account_holder_name(self, account_holder_name):
+    def set_account_holder_name(self, account_holder_name: Optional[str]) -> None:
         """
         Set method for to account_holder_name
         :param account_holder_name: account_holder_name
         """
         self.__account_holder_name = account_holder_name
 
-    def get_account_holder_address(self):
+    def get_account_holder_address(self) -> Optional[str]:
         """
         Get method for to account_holder_address
         :return: account_holder_address
         """
         return self.__account_holder_address
 
-    def set_account_holder_address(self, account_holder_address):
+    def set_account_holder_address(self, account_holder_address: Optional[str]) -> None:
         """
         Set method for to account_holder_address
         :param account_holder_address: account_holder_address
         """
         self.__account_holder_address = account_holder_address
 
-    def get_account_holder_address2(self):
+    def get_account_holder_address2(self) -> Optional[str]:
         """
         Get method for to account_holder_address2
         :return: account_holder_address2
         """
         return self.__account_holder_address2
 
-    def set_account_holder_address2(self, account_holder_address2):
+    def set_account_holder_address2(
+        self, account_holder_address2: Optional[str]
+    ) -> None:
         """
         Set method for to account_holder_address2
         :param account_holder_address2: account_holder_address2
         """
         self.__account_holder_address2 = account_holder_address2
 
-    def get_account_holder_postal_code(self):
+    def get_account_holder_postal_code(self) -> Optional[str]:
         """
         Get method for to account_holder_postal_code
         :return: account_holder_postal_code
         """
         return self.__account_holder_postal_code
 
-    def set_account_holder_postal_code(self, account_holder_postal_code):
+    def set_account_holder_postal_code(
+        self, account_holder_postal_code: Optional[str]
+    ) -> None:
         """
         Set method for to account_holder_postal_code
         :param account_holder_postal_code: account_holder_postal_code
         """
         self.__account_holder_postal_code = account_holder_postal_code
 
-    def get_account_holder_city(self):
+    def get_account_holder_city(self) -> Optional[str]:
         """
         Get method for to account_holder_city
         :return: account_holder_city
         """
         return self.__account_holder_city
 
-    def set_account_holder_city(self, account_holder_city):
+    def set_account_holder_city(self, account_holder_city: Optional[str]) -> None:
         """
         Set method for to account_holder_city
         :param account_holder_city: account_holder_city
         """
         self.__account_holder_city = account_holder_city
 
-    def get_account_holder_country(self):
+    def get_account_holder_country(self) -> Optional[str]:
         """
         Get method for to account_holder_country
         :return: account_holder_country
         """
         return self.__account_holder_country
 
-    def set_account_holder_country(self, account_holder_country):
+    def set_account_holder_country(self, account_holder_country: Optional[str]) -> None:
         """
         Set method for to account_holder_country
         :param account_holder_country: account_holder_country
         """
         self.__account_holder_country = account_holder_country
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "label": self.get_label(),
-            "bankCountry": self.get_bank_country(),
-            "name": self.get_name(),
-            "bank": self.get_bank(),
-            "swift": self.get_swift(),
-            "address": self.get_address(),
-            "city": self.get_city(),
-            "postal": self.get_postal(),
-            "sort": self.get_sort(),
-            "wire": self.get_wire(),
-            "bankName": self.get_bank_name(),
-            "bankAddress": self.get_bank_address(),
-            "iban": self.get_iban(),
-            "additionalInformation": self.get_additional_information(),
-            "accountHolderName": self.get_account_holder_name(),
-            "accountHolderAddress": self.get_account_holder_address(),
-            "accountHolderAddress2": self.get_account_holder_address2(),
-            "accountHolderPostalCode": self.get_account_holder_postal_code(),
-            "accountHolderCity": self.get_account_holder_city(),
-            "accountHolderCountry": self.get_account_holder_country(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/subscription/subscription.py` & `bitpay-4.0.0/src/bitpay/models/payout/payout_recipient.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,155 +1,172 @@
 """
-Subscription: Subscriptions are repeat billing agreements with specific buyers.
-BitPay sends bill emails to buyers identified in active subscriptions according
-to the specified schedule.
+PayoutRecipient
 """
-from .bill_data import BillData
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
 
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
-class Subscription:
+
+class PayoutRecipient:
     """
-    Subscription
+    PayoutRecipient
     """
 
-    __id = None
+    __email = None
+    __label = None
+    __notification_url = None
+    __data = None
+
     __status = None
-    """
-     BillData
-    """
-    __bill_data = None
-    __schedule = None
-    __next_delivery = None
-    __created_date = None
+    __id = None
+    __shopper_id = None
     __token = None
+    __guid = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
-                if key in ["billData"]:
-                    klass = globals()[key[0].upper() + key[1:]]
-
-                    if isinstance(value, list):
-                        objs = []
-                        for obj in value:
-                            objs.append(klass(**obj))
-                        value = objs
-                    else:
-                        value = klass(**value)
-                getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
+                if key == "notificationURL":
+                    self.set_notification_url(str(value))
+                else:
+                    getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(
+                        value
+                    )
             except AttributeError:
                 pass
 
-    def get_id(self):
+    def get_email(self) -> Optional[str]:
         """
-        Get method for the id
-        :return: id
+        Get method for email
+        :return: email
         """
-        return self.__id
+        return self.__email
 
-    def set_id(self, id):
+    def set_email(self, email: Optional[str]) -> None:
         """
-        Set method for to id
-        :param id: id
+        Set method for to email
+        :param email: email
         """
-        self.__id = id
+        self.__email = email
 
-    def get_status(self):
+    def get_data(self) -> Optional[str]:
         """
-        Get method for the status
-        :return: status
+        Get method for data
+        :return: data
         """
-        return self.__status
+        return self.__data
 
-    def set_status(self, status):
+    def set_data(self, data: Optional[str]) -> None:
         """
-        Set method for to status
-        :param status: status
+        Set method for to data
+        :param data: data
         """
-        self.__status = status
+        self.__data = data
+
+    def get_label(self) -> Optional[str]:
+        """
+        Get method for to label
+        :return: label
+        """
+        return self.__label
 
-    def get_bill_data(self):
+    def set_label(self, label: Optional[str]) -> None:
         """
-        Get method for the bill_data
-        :return: bill_data
+        Set method for to label
+        :param label: label
         """
-        return self.__bill_data
+        self.__label = label
 
-    def set_bill_data(self, bill_data: BillData):
+    def get_notification_url(self) -> Optional[str]:
         """
-        Set method for to bill_data
-        :param bill_data: bill_data
+        Get method for to notification_url
+        :return: notification_url
         """
-        self.__bill_data = bill_data
+        return self.__notification_url
 
-    def get_schedule(self):
+    def set_notification_url(self, notification_url: Optional[str]) -> None:
         """
-        Get method for the schedule
-        :return: schedule
+        Set method for to notification_url
+        :param notification_url: notification_url
         """
-        return self.__schedule
+        self.__notification_url = notification_url
 
-    def set_schedule(self, schedule):
+    def get_status(self) -> Optional[str]:
         """
-        Set method for to schedule
-        :param schedule: schedule
+        Get method for status
+        :return: status
         """
-        self.__schedule = schedule
+        return self.__status
 
-    def get_next_delivery(self):
+    def set_status(self, status: Optional[str]) -> None:
         """
-        Get method for the next_delivery
-        :return: next_delivery
+        Set method for status
+        :param status: status
         """
-        return self.__next_delivery
+        self.__status = status
+
+    def get_id(self) -> Optional[str]:
+        """
+        Get method for id
+        :return: id
+        """
+        return self.__id
 
-    def set_next_delivery(self, next_delivery):
+    def set_id(self, id: Optional[str]) -> None:
         """
-        Set method for to next_delivery
-        :param next_delivery: next_delivery
+        Set method for id
+        :param id: id
         """
-        self.__next_delivery = next_delivery
+        self.__id = id
 
-    def get_created_date(self):
+    def get_shopper_id(self) -> Optional[str]:
         """
-        Get method for the created_date
-        :return: created_date
+        Get method for to shopper_id
+        :return: shopper_id
         """
-        return self.__created_date
+        return self.__shopper_id
 
-    def set_created_date(self, created_date):
+    def set_shopper_id(self, shopper_id: Optional[str]) -> None:
         """
-        Set method for to created_date
-        :param created_date: created_date
+        Set method for to shopper_id
+        :param shopper_id: shopper_id
         """
-        self.__created_date = created_date
+        self.__shopper_id = shopper_id
 
-    def get_token(self):
+    def get_token(self) -> Optional[str]:
         """
-        Get method for the token
+        Get method for to token
         :return: token
         """
         return self.__token
 
-    def set_token(self, token):
+    def set_token(self, token: Optional[str]) -> None:
         """
         Set method for to token
         :param token: token
         """
         self.__token = token
 
-    def to_json(self):
+    def get_guid(self) -> Optional[str]:
+        """
+        Gets guid.
+        :return: guid
+        """
+        return self.__guid
+
+    def set_guid(self, value: Optional[str]) -> None:
+        """
+        Sets guid.
+        :param value: guid
+        """
+        self.__guid = value
+
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "id": self.get_id(),
-            "status": self.get_status(),
-            "billData": self.get_bill_data().to_json(),
-            "schedule": self.get_schedule(),
-            "nextDelivery": self.get_next_delivery(),
-            "createdDate": self.get_created_date(),
-            "token": self.get_token(),
-        }
-        data = {key: value for key, value in data.items() if value}
+        data = ModelUtil.to_json(self)
+        if "notificationUrl" in data:
+            data["notificationURL"] = data.pop("notificationUrl")
+
         return data
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/subscription/bill_data.py` & `bitpay-4.0.0/src/bitpay/models/settlement/settlement.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,324 +1,305 @@
 """
-BIll Data
+Settlement: Settlements are transfers of payment profits from BitPay to bank
+accounts and cryptocurrency wallets owned by merchants, partners, etc. This
+endpoint exposes reports detailing these settlements.
 """
-from .item import Item
-from ..currency import Currency
-from ...exceptions.bitpay_exception import BitPayException
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import List, Optional
 
+from .payout_info import PayoutInfo
+from .with_holdings import WithHoldings
+from .settlement_ledger_entry import SettlementLedgerEntry
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
-class BillData:
+
+class Settlement:
     """
-    Bill Data
+    Settlement
     """
 
-    __email_bill = None
-    __cc = None
-    __number = None
+    __id = None
+    __account_id = None
     __currency = None
-    __name = None
-    __address1 = None
-    __address2 = None
-    __city = None
-    __state = None
-    __zip = None
-    __country = None
-    __email = None
-    __phone = None
-    __due_date = None
-    __pass_processing_fee = None
-    __items = None
-    __merchant = None
-
-    def __init__(self, currency, email, due_date=None, **kwargs):
-        if currency:
-            self.set_currency(currency)
-        self.set_email(email)
-        self.set_due_date(due_date)
+    __payout_info = None
+    __status = None
+    __date_created = None
+    __date_executed = None
+    __date_completed = None
+    __opening_date = None
+    __closing_date = None
+    __opening_balance = None
+    __ledger_entries_sum = None
+    __withholdings = None
+    __withholdings_sum = None
+    __total_amount = None
+    __ledger_entries: Optional[List[SettlementLedgerEntry]] = None
+    __token = None
+    __amount_usd_unlocked = None
 
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
-                if key in ["items"]:
-                    klass = (
-                        Item if key == "items" else globals()[key[0].upper() + key[1:]]
-                    )
-
-                    if isinstance(value, list):
-                        objs = []
-                        for obj in value:
-                            objs.append(klass(**obj))
-                        value = objs
-                    else:
-                        value = klass(**value)
+                value = ModelUtil().get_field_value(
+                    key,
+                    value,
+                    {
+                        "payoutInfo": PayoutInfo,
+                        "openingBalance": "float",
+                        "ledgerEntriesSum": "float",
+                        "withHoldingsSum": "float",
+                        "totalAmount": "float",
+                    },
+                    {
+                        "withholdings": WithHoldings,
+                        "ledgerEntries": SettlementLedgerEntry,
+                    },
+                )
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_email_bill(self):
+    def get_id(self) -> Optional[str]:
         """
-        Get method for the email_bill
-        :return: email_bill
+        Get method for to id
+        :return: id
         """
-        return self.__email_bill
+        return self.__id
 
-    def set_email_bill(self, email_bill):
+    def set_id(self, id: Optional[str]) -> None:
         """
-        Set method for the email_bill
-        :param email_bill: email_bill
+        Set method for to id
+        :param id: id
         """
-        self.__email_bill = email_bill
+        self.__id = id
 
-    def get_cc(self):
+    def get_account_id(self) -> Optional[str]:
         """
-        Get method for the cc
-        :return: cc
+        Get method for to account_id
+        :return: account_id
         """
-        return self.__cc
+        return self.__account_id
 
-    def set_cc(self, cc):
+    def set_account_id(self, account_id: Optional[str]) -> None:
         """
-        Set method for the cc
-        :param cc: cc
+        Set method for to account_id
+        :param account_id: account_id
         """
-        self.__cc = cc
+        self.__account_id = account_id
 
-    def get_number(self):
+    def get_currency(self) -> Optional[str]:
         """
-        Get method for the number
-        :return: number
+        Get method for to currency
+        :return: currency
         """
-        return self.__number
+        return self.__currency
 
-    def set_number(self, number):
+    def set_currency(self, currency: Optional[str]) -> None:
         """
-        Set method for the number
-        :param number: number
+        Set method for to currency
+        :param currency: currency
         """
-        self.__number = number
+        self.__currency = currency
 
-    def get_currency(self):
+    def get_payout_info(self) -> Optional[PayoutInfo]:
         """
-        Get method for the currency
-        :return: currency
+        Get method for to payout_info
+        :return: payout_info
         """
-        return self.__currency
+        return self.__payout_info
 
-    def set_currency(self, currency):
+    def set_payout_info(self, payout_info: Optional[PayoutInfo]) -> None:
         """
-        Set method for the currency
-        :param currency: currency
+        Set method for to payout_info
+        :param payout_info: payout_info
         """
-        if not Currency.is_valid(currency):
-            raise BitPayException("currency code must be a type of Model.Currency")
-        self.__currency = currency
+        self.__payout_info = payout_info
 
-    def get_name(self):
+    def get_status(self) -> Optional[str]:
         """
-        Get method for the name
-        :return: name
+        Get method for to status
+        :return: status
         """
-        return self.__name
+        return self.__status
 
-    def set_name(self, name):
+    def set_status(self, status: Optional[str]) -> None:
         """
-        Set method for the name
-        :param name: name
+        Set method for to status
+        :param status: status
         """
-        self.__name = name
+        self.__status = status
 
-    def get_address1(self):
+    def get_date_created(self) -> Optional[str]:
         """
-        Get method for the address1
-        :return: address1
+        Get method for to date_created
+        :return: date_created
         """
-        return self.__address1
+        return self.__date_created
 
-    def set_address1(self, address1):
+    def set_date_created(self, date_created: Optional[str]) -> None:
         """
-        Set method for the address1
-        :param address1: address1
+        Set method for to date_created
+        :param date_created: date_created
         """
-        self.__address1 = address1
+        self.__date_created = date_created
 
-    def get_address2(self):
+    def get_date_executed(self) -> Optional[str]:
         """
-        Get method for the address2
-        :return: address2
+        Get method for to date_executed
+        :return: date_executed
         """
-        return self.__address2
+        return self.__date_executed
 
-    def set_address2(self, address2):
+    def set_date_executed(self, date_executed: Optional[str]) -> None:
         """
-        Set method for the address2
-        :param address2: address2
+        Set method for to date_executed
+        :param date_executed: date_executed
         """
-        self.__address2 = address2
+        self.__date_executed = date_executed
 
-    def get_city(self):
+    def get_date_completed(self) -> Optional[str]:
         """
-        Get method for the city
-        :return: city
+        Get method for to date_completed
+        :return: date_completed
         """
-        return self.__city
+        return self.__date_completed
 
-    def set_city(self, city):
+    def set_date_completed(self, date_completed: Optional[str]) -> None:
         """
-        Set method for the city
-        :param city: city
+        Set method for to date_completed
+        :param date_completed: date_completed
         """
-        self.__city = city
+        self.__date_completed = date_completed
 
-    def get_state(self):
+    def get_opening_date(self) -> Optional[str]:
         """
-        Get method for the state
-        :return: state
+        Get method for to opening_date
+        :return: opening_date
         """
-        return self.__state
+        return self.__opening_date
 
-    def set_state(self, state):
+    def set_opening_date(self, opening_date: Optional[str]) -> None:
         """
-        Set method for the state
-        :param state: state
+        Set method for to opening_date
+        :param opening_date: opening_date
         """
-        self.__state = state
+        self.__opening_date = opening_date
 
-    def get_zip(self):
+    def get_closing_date(self) -> Optional[str]:
         """
-        Get method for the zip
-        :return: zip
+        Get method for to closing_date
+        :return: closing_date
         """
-        return self.__zip
+        return self.__closing_date
 
-    def set_zip(self, zip):
+    def set_closing_date(self, closing_date: Optional[str]) -> None:
         """
-        Set method for the zip
-        :param zip: zip
+        Set method for to closing_date
+        :param closing_date: closing_date
         """
-        self.__zip = zip
+        self.__closing_date = closing_date
 
-    def get_country(self):
+    def get_opening_balance(self) -> Optional[float]:
         """
-        Get method for the country
-        :return: country
+        Get method for to opening_balance
+        :return: opening_balance
         """
-        return self.__country
+        return self.__opening_balance
 
-    def set_country(self, country):
+    def set_opening_balance(self, opening_balance: Optional[float]) -> None:
         """
-        Set method for the country
-        :param country: country
+        Set method for to opening_balance
+        :param opening_balance: opening_balance
         """
-        self.__country = country
+        self.__opening_balance = opening_balance
 
-    def get_email(self):
+    def get_ledger_entries_sum(self) -> Optional[float]:
         """
-        Get method for the email
-        :return: email
+        Get method for to ledger_entries_sum
+        :return: ledger_entries_sum
         """
-        return self.__email
+        return self.__ledger_entries_sum
 
-    def set_email(self, email):
+    def set_ledger_entries_sum(self, ledger_entries_sum: Optional[float]) -> None:
         """
-        Set method for the email
-        :param email: email
+        Set method for to ledger_entries_sum
+        :param ledger_entries_sum: ledger_entries_sum
         """
-        self.__email = email
+        self.__ledger_entries_sum = ledger_entries_sum
 
-    def get_phone(self):
+    def get_withholdings(self) -> Optional[List[WithHoldings]]:
         """
-        Get method for the phone
-        :return: phone
+        Get method for to withholdings
+        :return: List[WithHoldings]
         """
-        return self.__phone
+        return self.__withholdings
 
-    def set_phone(self, phone):
+    def set_withholdings(self, withholdings: List[WithHoldings]) -> None:
         """
-        Set method for the phone
-        :param phone: phone
+        Set method for to withholdings
+        :param withholdings: withholdings
         """
-        self.__phone = phone
+        self.__withholdings = withholdings
 
-    def get_due_date(self):
+    def get_withholdings_sum(self) -> Optional[float]:
         """
-        Get method for the due_date
-        :return: due_date
+        Get method for to withholdings_sum
+        :return: withholdings_sum
         """
-        return self.__due_date
+        return self.__withholdings_sum
 
-    def set_due_date(self, due_date):
+    def set_withholdings_sum(self, withholdings_sum: Optional[float]) -> None:
         """
-        Set method for the due_date
-        :param due_date: due_date
+        Set method for to withholdings_sum
+        :param withholdings_sum: withholdings_sum
         """
-        self.__due_date = due_date
+        self.__withholdings_sum = withholdings_sum
 
-    def get_pass_processing_fee(self):
+    def get_total_amount(self) -> Optional[float]:
         """
-        Get method for the pass_processing_fee
-        :return: pass_processing_fee
+        Get method for to total_amount
+        :return: total_amount
         """
-        return self.__pass_processing_fee
+        return self.__total_amount
 
-    def set_pass_processing_fee(self, pass_processing_fee):
+    def set_total_amount(self, total_amount: Optional[float]) -> None:
         """
-        Set method for the pass_processing_fee
-        :param pass_processing_fee: pass_processing_fee
+        Set method for to total_amount
+        :param total_amount: total_amount
         """
-        self.__pass_processing_fee = pass_processing_fee
+        self.__total_amount = total_amount
 
-    def get_items(self):
+    def get_ledger_entries(self) -> Optional[List[SettlementLedgerEntry]]:
         """
-        Get method for the items
-        :return: items
+        Get method for to ledger_entries
+        :return: ledger_entries
         """
-        return self.__items
+        return self.__ledger_entries
 
-    def set_items(self, items: [Item]):
+    def set_ledger_entries(
+        self, ledger_entries: Optional[List[SettlementLedgerEntry]]
+    ) -> None:
         """
-        Set method for the items
-        :param items: items
+        Set method for to ledger_entries
+        :param ledger_entries: ledger_entries
         """
-        self.__items = items
+        self.__ledger_entries = ledger_entries
 
-    def get_merchant(self):
+    def get_token(self) -> Optional[str]:
         """
-        Get method for the merchant
-        :return: merchant
+        Get method for to token
+        :return: token
         """
-        return self.__merchant
+        return self.__token
 
-    def set_merchant(self, merchant):
+    def set_token(self, token: Optional[str]) -> None:
         """
-        Set method for the merchant
-        :param merchant: merchant
+        Set method for to token
+        :param token: token
         """
-        self.__merchant = merchant
+        self.__token = token
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        items = []
-        for item in self.get_items():
-            items.append(item.to_json())
-        data = {
-            "emailBill": self.get_email_bill(),
-            "cc": self.get_cc(),
-            "number": self.get_number(),
-            "currency": self.get_currency(),
-            "name": self.get_name(),
-            "address1": self.get_address1(),
-            "address2": self.get_address2(),
-            "city": self.get_city(),
-            "state": self.get_state(),
-            "zip": self.get_zip(),
-            "country": self.get_country(),
-            "email": self.get_email(),
-            "phone": self.get_phone(),
-            "dueDate": self.get_due_date(),
-            "passProcessingFee": self.get_pass_processing_fee(),
-            "items": items,
-            "merchant": self.get_merchant(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/wallet/wallet.py` & `bitpay-4.0.0/src/bitpay/models/wallet/wallet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,121 @@
+from typing import List, Optional
+
 from .currencies import Currencies
-from ...utils import key_utils
+from bitpay.utils import key_utils
+from bitpay.utils.model_util import ModelUtil
+from bitpay.utils.model_util import ModelUtil
 
 
 class Wallet(object):
     """
     supported wallets and supported currency details
     """
 
     __key = None
     __display_name = None
     __avatar = None
     __pay_pro = None
-    __currencies = Currencies()
+    __currencies: Optional[List[Currencies]] = None
+    __image = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
-                if key in ["currencies"]:
-
-                    klass = globals()[key[0].upper() + key[1:]]
-
-                    if isinstance(value, list):
-                        objs = []
-                        for obj in value:
-                            objs.append(klass(**obj))
-                        value = objs
-                    else:
-                        value = klass(**value)
+                value = ModelUtil.get_field_value(
+                    key, value, {"payPro": "bool"}, {"currencies": Currencies}
+                )
                 getattr(
                     self, "set_%s" % key_utils.change_camel_case_to_snake_case(key)
                 )(value)
             except AttributeError:
                 pass
 
-    def get_key(self):
+    def get_key(self) -> Optional[str]:
         """
         Get method for to key
         :return: key
         """
         return self.__key
 
-    def set_key(self, key):
+    def set_key(self, key: Optional[str]) -> None:
         """
         Set method for to key
         :param key: key
         """
         self.__key = key
 
-    def get_display_name(self):
+    def get_display_name(self) -> Optional[str]:
         """
         Get method for to display_name
         :return: display_name
         """
         return self.__display_name
 
-    def set_display_name(self, display_name):
+    def set_display_name(self, display_name: Optional[str]) -> None:
         """
         Set method for to display_name
         :param display_name: display_name
         """
         self.__display_name = display_name
 
-    def get_avatar(self):
+    def get_avatar(self) -> Optional[str]:
         """
         Get method for to avatar
         :return: avatar
         """
         return self.__avatar
 
-    def set_avatar(self, avatar):
+    def set_avatar(self, avatar: Optional[str]) -> None:
         """
         Set method for to avatar
         :param avatar: avatar
         """
         self.__avatar = avatar
 
-    def get_pay_pro(self):
+    def get_pay_pro(self) -> Optional[bool]:
         """
         Get method for to paypro
         :return: paypro
         """
         return self.__paypro
 
-    def set_pay_pro(self, paypro):
+    def set_pay_pro(self, paypro: Optional[bool]) -> None:
         """
         Set method for to paypro
         :param paypro: paypro
         """
         self.__paypro = paypro
 
-    def get_currencies(self):
+    def get_currencies(self) -> Optional[List[Currencies]]:
         """
         Get method for to currencies
-        :return: currencies
+        :return: List[Currencies]
         """
         return self.__currencies
 
-    def set_currencies(self, currencies: Currencies):
+    def set_currencies(self, currencies: Optional[List[Currencies]]) -> None:
         """
         Set method for to currencies
         :param currencies: currencies
         """
         self.__currencies = currencies
 
-    def to_json(self):
+    def get_image(self) -> Optional[str]:
+        """
+        Get URL that displays wallet avatar image
+        :return: image
+        """
+        return self.__image
+
+    def set_image(self, value: Optional[str]) -> None:
+        """
+        Set URL that displays wallet avatar image
+        :param value: image
+        """
+        self.__image = value
+
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "key": self.get_key(),
-            "displayName": self.get_display_name(),
-            "avatar": self.get_avatar(),
-            "payPro": self.get_pay_pro(),
-            "currencies": self.get_currencies(),
-        }
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/currency.py` & `bitpay-4.0.0/src/bitpay/models/currency.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """
 Currency
 """
-from ..utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
+
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class Currency:
     """
     Currency: Crypto and fiat
     """
 
@@ -193,263 +196,185 @@
     ZAR = "ZAR"
     ZMW = "ZMW"
     ZWL = "ZWL"
 
     __code = None
     __symbol = None
     __precision = None
-    __currently_settled = None
     __name = None
     __plural = None
     __alts = None
     __minimum = None
-    __sanctioned = None
+    __sanctioned = False
     __decimals = None
-    __payout_fields = None
-    __settlement_minimum = None
     __chain = None
-    __tranche_decimals = None
-    __max_supply = None
 
     @classmethod
-    def is_valid(cls, value):
+    def is_valid(cls, value: str) -> bool:
         try:
             return hasattr(Currency(), value)
         except Exception:
             return False
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
+                value = ModelUtil.get_field_value(
+                    key,
+                    value,
+                    {
+                        "precision": "int",
+                        "minimum": "float",
+                        "sanctioned": "bool",
+                        "decimals": "int",
+                    },
+                    {},
+                )
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_code(self):
+    def get_code(self) -> Optional[str]:
         """
         Get method for to code
         :return: code
         """
         return self.__code
 
-    def set_code(self, code):
+    def set_code(self, code: Optional[str]) -> None:
         """
         Set method for to code
         :param code: code
         """
         self.__code = code
 
-    def get_symbol(self):
+    def get_symbol(self) -> Optional[str]:
         """
         Get method for to symbol
         :return: symbol
         """
         return self.__symbol
 
-    def set_symbol(self, symbol):
+    def set_symbol(self, symbol: Optional[str]) -> None:
         """
         Set method for to symbol
         :param symbol: symbol
         """
         self.__symbol = symbol
 
-    def get_chain(self):
+    def get_chain(self) -> Optional[str]:
         """
         Get method for to chain
         :return: chain
         """
         return self.__chain
 
-    def set_chain(self, chain):
+    def set_chain(self, chain: Optional[str]) -> None:
         """
         Set method for to chain
         :param chain: chain
         """
         self.__chain = chain
 
-    def get_tranche_decimals(self):
-        """
-        Get method for to tranche_decimals
-        :return: tranche_decimals
-        """
-        return self.__tranche_decimals
-
-    def set_tranche_decimals(self, tranche_decimals):
-        """
-        Set method for to tranche_decimals
-        :param tranche_decimals: tranche_decimals
-        """
-        self.__tranche_decimals = tranche_decimals
-
-    def get_max_supply(self):
-        """
-        Get method for to max_supply
-        :return: max_supply
-        """
-        return self.__max_supply
-
-    def set_max_supply(self, max_supply):
-        """
-        Set method for to max_supply
-        :param max_supply: max_supply
-        """
-        self.__max_supply = max_supply
-
-    def get_precision(self):
+    def get_precision(self) -> Optional[int]:
         """
         Get method for to precision
         :return: precision
         """
         return self.__precision
 
-    def set_precision(self, precision):
+    def set_precision(self, precision: Optional[int]) -> None:
         """
         Set method for to precision
         :param precision: precision
         """
         self.__precision = precision
 
-    def get_currently_settled(self):
-        """
-        Get method for to currently_settled
-        :return: currently_settled
-        """
-        return self.__currently_settled
-
-    def set_currently_settled(self, currently_settled):
-        """
-        Set method for to currently_settled
-        :param currently_settled: currently_settled
-        """
-        self.__currently_settled = currently_settled
-
-    def get_name(self):
+    def get_name(self) -> Optional[str]:
         """
         Get method for to name
         :return: name
         """
         return self.__name
 
-    def set_name(self, name):
+    def set_name(self, name: Optional[str]) -> None:
         """
         Set method for to name
         :param name: name
         """
         self.__name = name
 
-    def get_plural(self):
+    def get_plural(self) -> Optional[str]:
         """
         Get method for to plural
         :return: plural
         """
         return self.__plural
 
-    def set_plural(self, plural):
+    def set_plural(self, plural: Optional[str]) -> None:
         """
         Set method for to plural
         :param plural: plural
         """
         self.__plural = plural
 
-    def get_alts(self):
+    def get_alts(self) -> Optional[str]:
         """
         Get method for to alts
         :return: alts
         """
         return self.__alts
 
-    def set_alts(self, alts):
+    def set_alts(self, alts: Optional[str]) -> None:
         """
         Set method for to alts
         :param alts: alts
         """
         self.__alts = alts
 
-    def get_minimum(self):
+    def get_minimum(self) -> Optional[float]:
         """
         Get method for to minimum
         :return: minimum
         """
         return self.__minimum
 
-    def set_minimum(self, minimum):
+    def set_minimum(self, minimum: Optional[float]) -> None:
         """
         Set method for to minimum
         :param minimum: minimum
         """
         self.__minimum = minimum
 
-    def get_sanctioned(self):
+    def get_sanctioned(self) -> bool:
         """
         Get method for to sanctioned
         :return: sanctioned
         """
         return self.__sanctioned
 
-    def set_sanctioned(self, sanctioned):
+    def set_sanctioned(self, sanctioned: bool) -> None:
         """
         Set method for to sanctioned
         :param sanctioned: sanctioned
         """
         self.__sanctioned = sanctioned
 
-    def get_decimals(self):
+    def get_decimals(self) -> Optional[int]:
         """
         Get method for to decimals
         :return: decimals
         """
         return self.__decimals
 
-    def set_decimals(self, decimals):
+    def set_decimals(self, decimals: Optional[int]) -> None:
         """
         Set method for to decimals
         :param decimals: decimals
         """
         self.__decimals = decimals
 
-    def get_payout_fields(self):
-        """
-        Get method for to payout_fields
-        :return: payout_fields
-        """
-        return self.__payout_fields
-
-    def set_payout_fields(self, payout_fields):
-        """
-        Set method for to payout_fields
-        :param payout_fields: payout_fields
-        """
-        self.__payout_fields = payout_fields
-
-    def get_settlement_minimum(self):
-        """
-        Get method for to settlement_minimum
-        :return: settlement_minimum
-        """
-        return self.__settlement_minimum
-
-    def set_settlement_minimum(self, settlement_minimum):
-        """
-        Set method for to code
-        :param settlement_minimum: settlement_minimum
-        """
-        self.__settlement_minimum = settlement_minimum
-
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "code": self.get_code(),
-            "symbol": self.get_symbol(),
-            "precision": self.get_precision(),
-            "currentlySettled": self.get_currently_settled(),
-            "name": self.get_name(),
-            "plural": self.get_plural(),
-            "alts": self.get_alts(),
-            "minimum": self.get_minimum(),
-            "sanctioned": self.get_sanctioned(),
-            "decimals": self.get_decimals(),
-            "payoutFields": self.get_payout_fields(),
-            "settlementMinimum": self.get_settlement_minimum(),
-        }
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/payout/payout_recipients.py` & `bitpay-4.0.0/src/bitpay/models/payout/payout_recipients.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,76 @@
 """
 PayoutRecipients
 """
+from typing import Optional, List
+
 from .payout_recipient import PayoutRecipient
-from ...utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class PayoutRecipients:
     """
     PayoutRecipients
     """
 
-    __guid = ""
-    __recipients = []
-    __token = ""
+    __guid = None
+    __recipients: Optional[List[PayoutRecipient]] = None
+    __token = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
-                if key in [
-                    "recipients",
-                ]:
-                    klass = (
-                        PayoutRecipient
-                        if key == "recipients"
-                        else globals()[key[0].upper() + key[1:]]
-                    )
-                    if isinstance(value, list):
-                        objs = []
-                        for obj in value:
-                            objs.append(klass(**obj))
-                        value = objs
-                    else:
-                        value = klass(**value)
+                value = ModelUtil.get_field_value(
+                    key, value, {}, {"recipients": PayoutRecipient}
+                )
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_guid(self):
+    def get_guid(self) -> Optional[str]:
         """
         Get method for guid
         :return: guid
         """
         return self.__guid
 
-    def set_guid(self, guid):
+    def set_guid(self, guid: Optional[str]) -> None:
         """
         Set method for guid
         :param guid: guid
         """
         self.__guid = guid
 
-    def get_token(self):
+    def get_token(self) -> Optional[str]:
         """
         Get method for token
         :return: token
         """
         return self.__token
 
-    def set_token(self, token):
+    def set_token(self, token: Optional[str]) -> None:
         """
         Set method for token
         :param token: token
         """
         self.__token = token
 
-    def get_recipients(self):
+    def get_recipients(self) -> Optional[List[PayoutRecipient]]:
         """
         Get method for recipients
         :return: recipients
         """
         return self.__recipients
 
-    def set_recipients(self, recipients: [PayoutRecipient]):
+    def set_recipients(self, recipients: Optional[List[PayoutRecipient]]) -> None:
         """
         Set method for recipients
         :param recipients: recipients
         """
         self.__recipients = recipients
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        recipients = []
-        for recipient in self.get_recipients():
-            recipients.append(recipient.to_json())
-        data = {
-            "guid": self.get_guid(),
-            "token": self.get_token(),
-            "recipients": recipients,
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/payout/payout_instruction_transaction.py` & `bitpay-4.0.0/src/bitpay/models/settlement/with_holdings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,115 @@
-"""
-PayoutInstructionTransaction
-"""
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
 
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
-class PayoutInstructionTransaction:
+
+class WithHoldings:
     """
-    PayoutInstructionTransaction
+    Holdings
     """
 
-    __txid = None
     __amount = None
-    __date = None
-    __confirmations = None
+    __code = None
+    __description = None
+    __notes = None
+    __label = None
+    __bank_country = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
+            value = ModelUtil.get_field_value(key, value, {"amount": "float"}, {})
             try:
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_txid(self):
+    def get_amount(self) -> Optional[float]:
         """
-        Get method for txid
-        :return: txid
+        Get method for to amount
+        :return: amount
         """
-        return self.__txid
+        return self.__amount
 
-    def set_txid(self, txid):
+    def set_amount(self, amount: Optional[float]) -> None:
         """
-        Set method for to txid
-        :param txid: txid
+        Set method for to amount
+        :param amount: amount
         """
-        self.__txid = txid
+        self.__amount = amount
 
-    def get_confirmations(self):
+    def get_code(self) -> Optional[str]:
         """
-        Get method for confirmations
-        :return: confirmations
+        Get method for to code
+        :return: code
         """
-        return self.__confirmations
+        return self.__code
 
-    def set_confirmations(self, confirmations):
+    def set_code(self, code: Optional[str]) -> None:
         """
-        Set method for to confirmations
-        :param confirmations: confirmations
+        Set method for to code
+        :param code: code
         """
-        self.__confirmations = confirmations
+        self.__code = code
 
-    def get_amount(self):
+    def get_description(self) -> Optional[str]:
         """
-        Get method for amount
-        :return: amount
+        Get method for to description
+        :return: description
         """
-        return self.__amount
+        return self.__description
 
-    def set_amount(self, amount):
+    def set_description(self, description: Optional[str]) -> None:
         """
-        Set method for to amount
-        :param amount: amount
+        Set method for to description
+        :param description: description
         """
-        self.__amount = amount
+        self.__description = description
+
+    def get_notes(self) -> Optional[str]:
+        """
+        Get method for to notes
+        :return: notes
+        """
+        return self.__notes
+
+    def set_notes(self, notes: Optional[str]) -> None:
+        """
+        Set method for to notes
+        :param notes: notes
+        """
+        self.__notes = notes
+
+    def get_label(self) -> Optional[str]:
+        """
+        Get method for to label
+        :return: label
+        """
+        return self.__label
+
+    def set_label(self, label: Optional[str]) -> None:
+        """
+        Set method for to label
+        :param label: label
+        """
+        self.__label = label
 
-    def get_date(self):
+    def get_bank_country(self) -> Optional[str]:
         """
-        Get method for date
-        :return: date
+        Get method for to bank_country
+        :return: bank_country
         """
-        return self.__date
+        return self.__bank_country
 
-    def set_date(self, date):
+    def set_bank_country(self, bank_country: Optional[str]) -> None:
         """
-        Set method for to date
-        :param date: date
+        Set method for to bank_country
+        :param bank_country: bank_country
         """
-        self.__date = date
+        self.__bank_country = bank_country
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "txid": self.get_txid(),
-            "amount": self.get_amount(),
-            "date": self.get_date(),
-            "confirmations": self.get_confirmations(),
-        }
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/payout/payout.py` & `bitpay-4.0.0/src/bitpay/models/payout/payout.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,506 +1,428 @@
 """
 Payout
 """
-from ..currency import Currency
+from typing import Optional, List, Any, Dict
+
+from bitpay.models.currency import Currency
 from .payout_transaction import PayoutTransaction
-from ...exceptions.bitpay_exception import BitPayException
-from ...utils.key_utils import change_camel_case_to_snake_case
+from bitpay.exceptions.bitpay_exception import BitPayException
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class Payout:
     """
     Payout
     """
 
-    __token = ""
+    __token = None
 
     __amount = 0.0
-    __currency = ""
+    __currency = None
     __effective_date = None
 
-    __reference = ""
-    __notification_email = ""
-    __notification_url = ""
-    __redirect_url = ""
-    __ledger_currency = ""
+    __reference = None
+    __notification_email = None
+    __notification_url = None
+    __redirect_url = None
+    __ledger_currency = None
 
     __id = None
     __shopper_id = None
     __recipient_id = None
     __exchange_rates = None
     __account = None
     __email = None
     __label = None
     __support_phone = None
     __status = None
     __message = None
-    __percent_fee = None
-    __fee = None
-    __deposit_total = None
-    __rate = None
-    __btc = None
     __request_date = None
     __date_executed = None
-    __transactions = []
+    __transactions: Optional[List[PayoutTransaction]]
     __account_id = None
+    __group_id: Optional[str] = None
 
-    def __init__(self, amount=None, currency=None, ledger_currency=None, **kwargs):
+    def __init__(
+        self,
+        amount: float = 0.0,
+        currency: Optional[str] = None,
+        ledger_currency: Optional[str] = None,
+        **kwargs: Dict[str, Any]
+    ) -> None:
         self.set_amount(amount)
         if currency:
             self.set_currency(currency)
         if ledger_currency:
             self.set_ledger_currency(ledger_currency)
 
         for key, value in kwargs.items():
             try:
-                if key in ["transactions"]:
-                    if key == "transactions":
-                        klass = PayoutTransaction
-                    else:
-                        klass = globals()[key[0].upper() + key[1:]]
-
-                    if isinstance(value, list):
-                        objs = []
-                        for obj in value:
-                            objs.append(klass(**obj))
-                        value = objs
-                    else:
-                        value = klass(**value)
+                value = ModelUtil.get_field_value(
+                    key,
+                    value,
+                    {
+                        "amount": "float",
+                        "effectiveDate": "str",
+                        "requestDate": "str",
+                        "dateExecuted": "str",
+                        "code": "int",
+                    },
+                    {"exchangeRates": "dict", "transactions": PayoutTransaction},
+                )
+                if key in ["notificationURL"]:
+                    self.set_notification_url(str(value))
+                    continue
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_token(self):
+    def get_token(self) -> Optional[str]:
         """
         Get method for to token
         :return: token
         """
         return self.__token
 
-    def set_token(self, token):
+    def set_token(self, token: Optional[str]) -> None:
         """
         Set method for to token
         :param token: token
         """
         self.__token = token
 
-    def get_amount(self):
+    def get_amount(self) -> float:
         """
         Get method for to amount
         :return: amount
         """
         return self.__amount
 
-    def set_amount(self, amount):
+    def set_amount(self, amount: float) -> None:
         """
         Set method for to amount
         :param amount: amount
         """
         self.__amount = amount
 
-    def get_account_id(self):
+    def get_account_id(self) -> Optional[str]:
         """
         Get method for to account_id
         :return: account_id
         """
         return self.__account_id
 
-    def set_account_id(self, account_id):
+    def set_account_id(self, account_id: Optional[str]) -> None:
         """
         Set method for to account_id
         :param account_id: account_id
         """
         self.__account_id = account_id
 
-    def get_currency(self):
+    def get_currency(self) -> Optional[str]:
         """
         Get method for to currency
         :return: currency
         """
         return self.__currency
 
-    def set_currency(self, currency):
+    def set_currency(self, currency: str) -> None:
         """
         Set method for to currency
         :param currency: currency
         """
         if not Currency.is_valid(currency):
             raise BitPayException("currency code must be a type of Model.Currency")
         self.__currency = currency
 
-    def get_effective_date(self):
+    def get_effective_date(self) -> Optional[str]:
         """
         Get method for to effective_date
         :return: effective_date
         """
         return self.__effective_date
 
-    def set_effective_date(self, effective_date):
+    def set_effective_date(self, effective_date: Optional[str]) -> None:
         """
         Set method for to effective_date
         :param effective_date: effective_date
         """
         self.__effective_date = effective_date
 
-    def get_reference(self):
+    def get_reference(self) -> Optional[str]:
         """
         Get method for to reference
         :return: reference
         """
         return self.__reference
 
-    def set_reference(self, reference):
+    def set_reference(self, reference: Optional[str]) -> None:
         """
         Set method for to reference
         :param reference: reference
         """
         self.__reference = reference
 
-    def get_notification_email(self):
+    def get_notification_email(self) -> Optional[str]:
         """
         Get method for to notification_email
         :return: notification_email
         """
         return self.__notification_email
 
-    def set_notification_email(self, notification_email):
+    def set_notification_email(self, notification_email: Optional[str]) -> None:
         """
         Set method for to notification_email
         :param notification_email: notification_email
         """
         self.__notification_email = notification_email
 
-    def get_notification_url(self):
+    def get_notification_url(self) -> Optional[str]:
         """
         Get method for to notification_url
         :return: notification_url
         """
         return self.__notification_url
 
-    def set_notification_url(self, notification_url):
+    def set_notification_url(self, notification_url: Optional[str]) -> None:
         """
         Set method for to notification_url
         :param notification_url: notification_url
         """
         self.__notification_url = notification_url
 
-    def get_redirect_url(self):
+    def get_redirect_url(self) -> Optional[str]:
         """
         Get method for to redirect_url
         :return: redirect_url
         """
         return self.__redirect_url
 
-    def set_redirect_url(self, redirect_url):
+    def set_redirect_url(self, redirect_url: Optional[str]) -> None:
         """
         Set method for to redirect_url
         :param redirect_url: redirect_url
         """
         self.__redirect_url = redirect_url
 
-    def get_ledger_currency(self):
+    def get_ledger_currency(self) -> Optional[str]:
         """
         Get method for to ledger_currency
         :return: ledger_currency
         """
         return self.__ledger_currency
 
-    def set_ledger_currency(self, ledger_currency):
+    def set_ledger_currency(self, ledger_currency: str) -> None:
         """
         Set method for to ledger_currency
         :param ledger_currency: ledger_currency
         """
         if not Currency.is_valid(ledger_currency):
             raise BitPayException("currency code must be a type of Model.Currency")
         self.__ledger_currency = ledger_currency
 
-    def get_id(self):
+    def get_id(self) -> Optional[str]:
         """
         Get method for to id
         :return: id
         """
         return self.__id
 
-    def set_id(self, id):
+    def set_id(self, id: Optional[str]) -> None:
         """
         Set method for to id
         :param id: id
         """
         self.__id = id
 
-    def get_shopper_id(self):
+    def get_shopper_id(self) -> Optional[str]:
         """
         Get method for to shopper_id
         :return: shopper_id
         """
         return self.__shopper_id
 
-    def set_shopper_id(self, shopper_id):
+    def set_shopper_id(self, shopper_id: Optional[str]) -> None:
         """
         Set method for to shopper_id
         :param shopper_id: shopper_id
         """
         self.__shopper_id = shopper_id
 
-    def get_recipient_id(self):
+    def get_recipient_id(self) -> Optional[str]:
         """
         Get method for to recipient_id
         :return: recipient_id
         """
         return self.__recipient_id
 
-    def set_recipient_id(self, recipient_id):
+    def set_recipient_id(self, recipient_id: Optional[str]) -> None:
         """
         Set method for to recipient_id
         :param recipient_id: recipient_id
         """
         self.__recipient_id = recipient_id
 
-    def get_exchange_rates(self):
+    def get_exchange_rates(self) -> Optional[List[dict]]:
         """
         Get method for to exchange_rates
         :return: exchange_rates
         """
         return self.__exchange_rates
 
-    def set_exchange_rates(self, exchange_rates):
+    def set_exchange_rates(self, exchange_rates: Optional[List[dict]]) -> None:
         """
         Set method for to exchange_rates
         :param exchange_rates: exchange_rates
         """
         self.__exchange_rates = exchange_rates
 
-    def get_account(self):
+    def get_account(self) -> Optional[str]:
         """
         Get method for to account
         :return: account
         """
         return self.__account
 
-    def set_account(self, account):
+    def set_account(self, account: Optional[str]) -> None:
         """
         Set method for to account
         :param account: account
         """
         self.__account = account
 
-    def get_email(self):
+    def get_email(self) -> Optional[str]:
         """
         Get method for to email
         :return: email
         """
         return self.__email
 
-    def set_email(self, email):
+    def set_email(self, email: Optional[str]) -> None:
         """
         Set method for to email
         :param email: email
         """
         self.__email = email
 
-    def get_label(self):
+    def get_label(self) -> Optional[str]:
         """
         Get method for to label
         :return: label
         """
         return self.__label
 
-    def set_label(self, label):
+    def set_label(self, label: Optional[str]) -> None:
         """
         Set method for to label
         :param label: label
         """
         self.__label = label
 
-    def get_support_phone(self):
+    def get_support_phone(self) -> Optional[str]:
         """
         Get method for to support_phone
         :return: support_phone
         """
         return self.__support_phone
 
-    def set_support_phone(self, support_phone):
+    def set_support_phone(self, support_phone: Optional[str]) -> None:
         """
         Set method for to support_phone
         :param support_phone: support_phone
         """
         self.__support_phone = support_phone
 
-    def get_status(self):
+    def get_status(self) -> Optional[str]:
         """
         Get method for to status
         :return: status
         """
         return self.__status
 
-    def set_status(self, status):
+    def set_status(self, status: Optional[str]) -> None:
         """
         Set method for to status
         :param status: status
         """
         self.__status = status
 
-    def get_message(self):
+    def get_message(self) -> Optional[str]:
         """
         Get method for to message
         :return: message
         """
         return self.__message
 
-    def set_message(self, message):
+    def set_message(self, message: Optional[str]) -> None:
         """
         Set method for to message
         :param message: message
         """
         self.__message = message
 
-    def get_percent_fee(self):
-        """
-        Get method for to percent_fee
-        :return: percent_fee
-        """
-        return self.__percent_fee
-
-    def set_percent_fee(self, percent_fee):
-        """
-        Set method for to percent_fee
-        :param percent_fee: percent_fee
-        """
-        self.__percent_fee = percent_fee
-
-    def get_fee(self):
-        """
-        Get method for to fee
-        :return: fee
-        """
-        return self.__fee
-
-    def set_fee(self, fee):
-        """
-        Set method for to fee
-        :param fee: fee
-        """
-        self.__fee = fee
-
-    def get_deposit_total(self):
-        """
-        Get method for to deposit_total
-        :return: deposit_total
-        """
-        return self.__deposit_total
-
-    def set_deposit_total(self, deposit_total):
-        """
-        Set method for to deposit_total
-        :param deposit_total: deposit_total
-        """
-        self.__deposit_total = deposit_total
-
-    def get_rate(self):
-        """
-        Get method for to rate
-        :return: rate
-        """
-        return self.__rate
-
-    def set_rate(self, rate):
-        """
-        Set method for to rate
-        :param rate: rate
-        """
-        self.__rate = rate
-
-    def get_btc(self):
-        """
-        Get method for to btc
-        :return: btc
-        """
-        return self.__btc
-
-    def set_btc(self, btc):
-        """
-        Set method for to btc
-        :param btc: btc
-        """
-        self.__btc = btc
-
-    def get_request_date(self):
+    def get_request_date(self) -> Optional[str]:
         """
         Get method for to code
         :return: code
         """
         return self.__request_date
 
-    def set_request_date(self, request_date):
+    def set_request_date(self, request_date: Optional[str]) -> None:
         """
         Set method for to request_date
         :param request_date: request_date
         """
         self.__request_date = request_date
 
-    def get_date_executed(self):
+    def get_date_executed(self) -> Optional[str]:
         """
         Get method for to date_executed
         :return: date_executed
         """
         return self.__date_executed
 
-    def set_date_executed(self, date_executed):
+    def set_date_executed(self, date_executed: Optional[str]) -> None:
         """
         Set method for to date_executed
         :param date_executed: date_executed
         """
         self.__date_executed = date_executed
 
-    def get_transactions(self):
+    def get_transactions(self) -> Optional[List[PayoutTransaction]]:
         """
         Get method for to transactions
         :return: transactions
         """
         return self.__transactions
 
-    def set_transactions(self, transactions: [PayoutTransaction]):
+    def set_transactions(self, transactions: Optional[List[PayoutTransaction]]) -> None:
         """
         Set method for to transactions
         :param transactions: transactions
         """
         self.__transactions = transactions
 
-    def to_json(self):
+    def get_group_id(self) -> Optional[str]:
+        """
+        Added to the payouts made at the same time through the `Create Payout Group` request.
+        Can be used for querying or deleting.
+        """
+        return self.__group_id
+
+    def set_group_id(self, value: str) -> None:
+        """
+        Added to the payouts made at the same time through the `Create Payout Group` request.
+        Can be used for querying or deleting.
+        """
+        self.__group_id = value
+
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        transactions = []
-        for transaction in self.get_transactions():
-            transactions.append(transaction.to_json())
-        data = {
-            "token": self.get_token(),
-            "amount": self.get_amount(),
-            "currency": self.get_currency(),
-            "effectiveDate": self.get_effective_date(),
-            "ledgerCurrency": self.get_ledger_currency(),
-            "reference": self.get_reference(),
-            "notificationURL": self.get_notification_url(),
-            "notificationEmail": self.get_notification_email(),
-            "email": self.get_email(),
-            "recipientId": self.get_recipient_id(),
-            "shopperId": self.get_shopper_id(),
-            "label": self.get_label(),
-            "message": self.get_message(),
-            "id": self.get_id(),
-            "status": self.get_status(),
-            "requestDate": self.get_request_date(),
-            "exchangeRates": self.get_exchange_rates(),
-            "transactions": transactions,
-            "dateExecuted": self.get_date_executed(),
-            "rate": self.get_rate(),
-            "depositTotal": self.get_deposit_total(),
-            "fee": self.get_fee(),
-            "percentFee": self.get_percent_fee(),
-            "supportPhone": self.get_support_phone(),
-            "account": self.get_account(),
-            "redirectUrl": self.get_redirect_url(),
-            "btc": self.get_btc(),
-        }
-        data = {key: value for key, value in data.items() if value}
+        data = ModelUtil.to_json(self)
+        if "notificationUrl" in data:
+            data["notificationURL"] = data.pop("notificationUrl")
+
         return data
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/invoice/buyer_provided_info.py` & `bitpay-4.0.0/src/bitpay/models/invoice/buyer_provided_info.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,139 @@
 """
 BuyerProvidedInfo: Information collected from the buyer during the process of paying
 an invoice. Initially this object is empty.
 """
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Union, Optional
+
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class BuyerProvidedInfo:
     """
     Information collected from the buyer during the process of paying an invoice.
      Initially this object is empty.
     """
 
-    __name = ""
-    __phone_number = ""
-    __selected_wallet = ""
-    __email_address = ""
-    __selected_transaction_currency = ""
+    __name = None
+    __phone_number = None
+    __selected_wallet = None
+    __email_address = None
+    __selected_transaction_currency = None
+    __sms = None
+    __sms_verified = False
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
+                value = ModelUtil.get_field_value(
+                    key, value, {"smsVerified": "bool"}, {}
+                )
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_name(self):
+    def get_name(self) -> Optional[str]:
         """
         Get method for the name
         :return: name
         """
         return self.__name
 
-    def set_name(self, name):
+    def set_name(self, name: Optional[str]) -> None:
         """
         Set method for to name
         :param name: name
         """
         self.__name = name
 
-    def get_phone_number(self):
+    def get_phone_number(self) -> Optional[str]:
         """
         Get method for the phone_number
         :return: phone_number
         """
         return self.__phone_number
 
-    def set_phone_number(self, phone_number):
+    def set_phone_number(self, phone_number: Optional[str]) -> None:
         """
         Set method for to phone_number
         :param phone_number: phone_number
         """
         self.__phone_number = phone_number
 
-    def get_selected_wallet(self):
+    def get_selected_wallet(self) -> Optional[str]:
         """
         Get method for the selected_wallet
         :return: selected_wallet
         """
         return self.__selected_wallet
 
-    def set_selected_wallet(self, selected_wallet):
+    def set_selected_wallet(self, selected_wallet: Optional[str]) -> None:
         """
         Set method for to selected_wallet
         :param selected_wallet: selected_wallet
         """
         self.__selected_wallet = selected_wallet
 
-    def get_email_address(self):
+    def get_email_address(self) -> Optional[str]:
         """
         Get method for the email_address
         :return: email_address
         """
         return self.__email_address
 
-    def set_email_address(self, email_address):
+    def set_email_address(self, email_address: Optional[str]) -> None:
         """
         Set method for to email_address
         :param email_address: email_address
         """
         self.__email_address = email_address
 
-    def get_selected_transaction_currency(self):
+    def get_selected_transaction_currency(self) -> Optional[str]:
         """
         Get method for the selected_transaction_currency
         :return: selected_transaction_currency
         """
         return self.__selected_transaction_currency
 
-    def set_selected_transaction_currency(self, selected_transaction_currency):
+    def set_selected_transaction_currency(
+        self, selected_transaction_currency: Optional[str]
+    ) -> None:
         """
         Set method for to selected_transaction_currency
         :param selected_transaction_currency: selected_transaction_currency
         """
         self.__selected_transaction_currency = selected_transaction_currency
 
-    def to_json(self):
+    def get_sms(self) -> Optional[str]:
+        """
+        Get sms
+        :return: Union[str, None]
+        """
+        return self.__sms
+
+    def get_sms_verified(self) -> bool:
+        """
+        Get sms verified
+        :return: bool
+        """
+        return self.__sms_verified
+
+    def set_sms(self, value: Optional[str]) -> None:
+        """
+        Set sms
+        :param value: str
+        """
+        self.__sms = value
+
+    def set_sms_verified(self, value: bool) -> None:
+        """
+        Set sms verified
+        :param value: bool
+        """
+        self.__sms_verified = value
+
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "name": self.get_name(),
-            "phoneNumber": self.get_phone_number(),
-            "selectedWallet": self.get_selected_wallet(),
-            "emailAddress": self.get_email_address(),
-            "selectedTransactionCurrency": self.get_selected_transaction_currency(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/invoice/buyer.py` & `bitpay-4.0.0/src/bitpay/models/invoice/buyer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,203 +1,193 @@
 """
 Buyer
 """
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
+
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class Buyer:
     """
     Allows merchant to pass buyer related information in the invoice object
     """
 
-    __name = ""
-    __address1 = ""
-    __address2 = ""
-    __locality = ""
-    __region = ""
-    __postal_code = ""
-    __country = ""
-    __email = ""
-    __phone = ""
-    __notify = ""
-    __buyer_email = ""
+    __name = None
+    __address1 = None
+    __address2 = None
+    __locality = None
+    __region = None
+    __postal_code = None
+    __country = None
+    __email = None
+    __phone = None
+    __notify = False
+    __buyer_email = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
+                value = ModelUtil.get_field_value(key, value, {"notify": "bool"}, {})
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_name(self):
+    def get_name(self) -> Optional[str]:
         """
         Get method for the name
         :return: name
         """
         return self.__name
 
-    def set_name(self, name):
+    def set_name(self, name: Optional[str]) -> None:
         """
         Set method for the name
         :param name: name
         """
         self.__name = name
 
-    def get_buyer_email(self):
+    def get_buyer_email(self) -> Optional[str]:
         """
         Get method for the buyer_email
         :return: buyer_email
         """
         return self.__buyer_email
 
-    def set_buyer_email(self, buyer_email):
+    def set_buyer_email(self, buyer_email: Optional[str]) -> None:
         """
         Set method for the buyer_email
         :param buyer_email: buyer_email
         """
         self.__buyer_email = buyer_email
 
-    def get_address1(self):
+    def get_address1(self) -> Optional[str]:
         """
         Get method for the address1
         :return: address1
         """
         return self.__address1
 
-    def set_address1(self, address1):
+    def set_address1(self, address1: Optional[str]) -> None:
         """
         Set method for the address1
         :param address1: address1
         """
         self.__address1 = address1
 
-    def get_address2(self):
+    def get_address2(self) -> Optional[str]:
         """
         Get method for the address2
         :return: address2
         """
         return self.__address2
 
-    def set_address2(self, address2):
+    def set_address2(self, address2: Optional[str]) -> None:
         """
         Set method for the address2
         :param address2: address2
         """
         self.__address2 = address2
 
-    def get_locality(self):
+    def get_locality(self) -> Optional[str]:
         """
         Get method for the locality
         :return: locality
         """
         return self.__locality
 
-    def set_locality(self, locality):
+    def set_locality(self, locality: Optional[str]) -> None:
         """
         Set method for the locality
         :param locality: locality
         """
         self.__locality = locality
 
-    def get_region(self):
+    def get_region(self) -> Optional[str]:
         """
         Get method for the region
         :return: region
         """
         return self.__region
 
-    def set_region(self, region):
+    def set_region(self, region: Optional[str]) -> None:
         """
         Set method for the region
         :param region: region
         """
         self.__region = region
 
-    def get_postal_code(self):
+    def get_postal_code(self) -> Optional[str]:
         """
         Get method for the postal_code
         :return: postal_code
         """
         return self.__postal_code
 
-    def set_postal_code(self, postal_code):
+    def set_postal_code(self, postal_code: Optional[str]) -> None:
         """
         Set method for the postal_code
         :param postal_code: postal_code
         """
         self.__postal_code = postal_code
 
-    def get_country(self):
+    def get_country(self) -> Optional[str]:
         """
         Get method for the country
         :return: country
         """
         return self.__country
 
-    def set_country(self, country):
+    def set_country(self, country: Optional[str]) -> None:
         """
         Set method for the country
         :param country: country
         """
         self.__country = country
 
-    def get_email(self):
+    def get_email(self) -> Optional[str]:
         """
         Get method for the email
         :return: email
         """
         return self.__email
 
-    def set_email(self, email):
+    def set_email(self, email: Optional[str]) -> None:
         """
         Set method for the email
         :param email: email
         """
         self.__email = email
 
-    def get_phone(self):
+    def get_phone(self) -> Optional[str]:
         """
         Get method for the phone
         :return: phone
         """
         return self.__phone
 
-    def set_phone(self, phone):
+    def set_phone(self, phone: Optional[str]) -> None:
         """
         Set method for the phone
         :param phone: phone
         """
         self.__phone = phone
 
-    def get_notify(self):
+    def get_notify(self) -> bool:
         """
         Get method for to notify
         :return: notify
         """
         return self.__notify
 
-    def set_notify(self, notify):
+    def set_notify(self, notify: bool = False) -> None:
         """
         Set method for to notify
         :param notify: notify
         """
         self.__notify = notify
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "name": self.get_name(),
-            "address1": self.get_address1(),
-            "address2": self.get_address2(),
-            "locality": self.get_locality(),
-            "region": self.get_region(),
-            "postalCode": self.get_postal_code(),
-            "country": self.get_country(),
-            "email": self.get_email(),
-            "phone": self.get_phone(),
-            "notify": self.get_notify(),
-            "buyerEmail": self.get_buyer_email(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/invoice/supported_transaction_currencies.py` & `bitpay-4.0.0/src/bitpay/models/invoice/supported_transaction_currencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """
 SupportedTransactionCurrencies
 """
+from typing import Optional, Dict, Any
+
 from .supported_transaction_currency import SupportedTransactionCurrency
+from bitpay.utils.model_util import ModelUtil
 
 
 class SupportedTransactionCurrencies:
     """
     currency selected for payment
     """
 
@@ -16,185 +19,174 @@
     __gusd = SupportedTransactionCurrency()
     __busd = SupportedTransactionCurrency()
     __pax = SupportedTransactionCurrency()
     __xrp = SupportedTransactionCurrency()
     __doge = SupportedTransactionCurrency()
     __ltc = SupportedTransactionCurrency()
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Dict[str, Any]) -> None:
         for key, value in kwargs.items():
             try:
                 if key in [
                     "BTC",
                     "BCH",
                     "ETH",
                     "USDC",
                     "GUSD",
                     "BUSD",
                     "PAX",
                     "XRP",
                     "DOGE",
                     "LTC",
                 ]:
-                    value = SupportedTransactionCurrency(**value)
+                    if not isinstance(value, SupportedTransactionCurrency):
+                        value = dict(value)
+                        value = SupportedTransactionCurrency(**value)  # type: ignore
                 getattr(self, "set_%s" % key.lower())(value)
             except AttributeError:
                 pass
 
-    def get_btc(self):
+    def get_btc(self) -> Optional[SupportedTransactionCurrency]:
         """
         Get method for to btc
         :return: btc
         """
         return self.__btc
 
-    def set_btc(self, btc: SupportedTransactionCurrency):
+    def set_btc(self, btc: SupportedTransactionCurrency) -> None:
         """
         Set method for to btc
         :param btc: btc
         """
         self.__btc = btc
 
-    def get_bch(self):
+    def get_bch(self) -> Optional[SupportedTransactionCurrency]:
         """
         Get method for to bch
         :return: bch
         """
         return self.__bch
 
-    def set_bch(self, bch: SupportedTransactionCurrency):
+    def set_bch(self, bch: SupportedTransactionCurrency) -> None:
         """
         Set method for to bch
         :param bch: bch
         """
         self.__bch = bch
 
-    def get_eth(self):
+    def get_eth(self) -> Optional[SupportedTransactionCurrency]:
         """
         Get method for to eth
         :return: eth
         """
         return self.__eth
 
-    def set_eth(self, eth: SupportedTransactionCurrency):
+    def set_eth(self, eth: SupportedTransactionCurrency) -> None:
         """
         Set method for to eth
         :param eth: eth
         """
         self.__eth = eth
 
-    def get_usdc(self):
+    def get_usdc(self) -> Optional[SupportedTransactionCurrency]:
         """
         Get method for to usdc
         :return: usdc
         """
         return self.__usdc
 
-    def set_usdc(self, usdc: SupportedTransactionCurrency):
+    def set_usdc(self, usdc: SupportedTransactionCurrency) -> None:
         """
         Set method for to usdc
         :param usdc: usdc
         """
         self.__usdc = usdc
 
-    def get_gusd(self):
+    def get_gusd(self) -> Optional[SupportedTransactionCurrency]:
         """
         Get method for to gusd
         :return: gusd
         """
         return self.__gusd
 
-    def set_gusd(self, gusd: SupportedTransactionCurrency):
+    def set_gusd(self, gusd: SupportedTransactionCurrency) -> None:
         """
         Set method for to gusd
         :param gusd: gusd
         """
         self.__gusd = gusd
 
-    def get_busd(self):
+    def get_busd(self) -> Optional[SupportedTransactionCurrency]:
         """
         Get method for to busd
         :return: busd
         """
         return self.__busd
 
-    def set_busd(self, busd: SupportedTransactionCurrency):
+    def set_busd(self, busd: SupportedTransactionCurrency) -> None:
         """
         Set method for to busd
-        :param user: busd
+        :param busd: busd
         """
         self.__busd = busd
 
-    def get_pax(self):
+    def get_pax(self) -> Optional[SupportedTransactionCurrency]:
         """
         Get method for to pax
         :return: pax
         """
         return self.__pax
 
-    def set_pax(self, pax: SupportedTransactionCurrency):
+    def set_pax(self, pax: SupportedTransactionCurrency) -> None:
         """
         Set method for to pax
         :param pax: pax
         """
         self.__pax = pax
 
-    def get_xrp(self):
+    def get_xrp(self) -> Optional[SupportedTransactionCurrency]:
         """
         Get method for to xrp
         :return: xrp
         """
         return self.__xrp
 
-    def set_xrp(self, xrp: SupportedTransactionCurrency):
+    def set_xrp(self, xrp: SupportedTransactionCurrency) -> None:
         """
         Set method for to xrp
         :param xrp: xrp
         """
         self.__xrp = xrp
 
-    def get_doge(self):
+    def get_doge(self) -> Optional[SupportedTransactionCurrency]:
         """
         Get method for to doge
         :return: doge
         """
         return self.__doge
 
-    def set_doge(self, doge: SupportedTransactionCurrency):
+    def set_doge(self, doge: SupportedTransactionCurrency) -> None:
         """
         Set method for to doge
         :param doge: doge
         """
         self.__doge = doge
 
-    def get_ltc(self):
+    def get_ltc(self) -> Optional[SupportedTransactionCurrency]:
         """
         Get method for to ltc
         :return: ltc
         """
         return self.__ltc
 
-    def set_ltc(self, ltc: SupportedTransactionCurrency):
+    def set_ltc(self, ltc: SupportedTransactionCurrency) -> None:
         """
         Set method for to ltc
         :param ltc: ltc
         """
         self.__ltc = ltc
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "btc": self.get_btc(),
-            "bch": self.get_bch(),
-            "eth": self.get_eth(),
-            "usdc": self.get_usdc(),
-            "gusd": self.get_gusd(),
-            "busd": self.get_busd(),
-            "pax": self.get_pax(),
-            "xrp": self.get_xrp(),
-            "doge": self.get_doge(),
-            "ltc": self.get_ltc(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/invoice/supported_transaction_currency.py` & `bitpay-4.0.0/src/bitpay/models/invoice/supported_transaction_currency.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 """
 SupportedTransactionCurrency
 """
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
+
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class SupportedTransactionCurrency:
     """
     currency selected for payment is enabled
     """
 
-    __enabled = None
+    __enabled = False
     __reason = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict):
         for key, value in kwargs.items():
             try:
+                value = ModelUtil.get_field_value(key, value, {"enabled": "bool"}, {})
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_enabled(self):
+    def get_enabled(self) -> bool:
         """
         Get method for to enabled
         :return: enabled
         """
         return self.__enabled
 
-    def set_enabled(self, enabled):
+    def set_enabled(self, enabled: bool) -> None:
         """
         Set method for to enabled
         :param enabled: enabled
         """
         self.__enabled = enabled
 
-    def get_reason(self):
+    def get_reason(self) -> Optional[str]:
         """
         Get method for to reason
         :return: reason
         """
         return self.__reason
 
-    def set_reason(self, reason):
+    def set_reason(self, reason: Optional[str]) -> None:
         """
         Set method for to reason
         :param reason: reason
         """
         self.__reason = reason
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         data in json
         :return:
         """
-        data = {"enabled": self.get_enabled(), "reason": self.get_reason()}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/invoice/miner_fees.py` & `bitpay-4.0.0/src/bitpay/models/invoice/miner_fees.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """
 MinerFees
 """
+from typing import Optional, Any
+
 from .miner_fees_item import MinerFeesItem
+from bitpay.utils.model_util import ModelUtil
 
 
 class MinerFees:
     """
     The total amount of fees that the purchaser will pay to cover BitPay's
      UTXO sweep cost for an invoice. The key is the currency and the value
      is an amount in satoshis. This is referenced as "Network Cost" on an
@@ -19,175 +22,161 @@
     __gusd = MinerFeesItem()
     __pax = MinerFeesItem()
     __doge = MinerFeesItem()
     __ltc = MinerFeesItem()
     __busd = MinerFeesItem()
     __xrp = MinerFeesItem()
 
-    def __init__(self, **kwargs):
-
+    def __init__(self, **kwargs: Any) -> None:
         for key, value in kwargs.items():
             try:
-                if key in ["BTC", "BCH", "ETH", "USDC", "GUSD", "PAX", "BUSD", "XRP"]:
+                if not isinstance(value, MinerFeesItem):
                     value = MinerFeesItem(**value)
                 getattr(self, "set_%s" % key.lower())(value)
             except AttributeError:
                 pass
 
-    def get_btc(self):
+    def get_btc(self) -> Optional[MinerFeesItem]:
         """
         Get method for the btc
         :return: btc
         """
         return self.__btc
 
-    def set_btc(self, btc: MinerFeesItem):
+    def set_btc(self, btc: MinerFeesItem) -> None:
         """
         Set method for the btc
         :param btc: btc
         """
         self.__btc = btc
 
-    def get_bch(self):
+    def get_bch(self) -> Optional[MinerFeesItem]:
         """
         Get method for the bch
         :return: bch
         """
         return self.__bch
 
-    def set_bch(self, bch: MinerFeesItem):
+    def set_bch(self, bch: MinerFeesItem) -> None:
         """
         Set method for the bch
         :param bch: bch
         """
         self.__bch = bch
 
-    def get_eth(self):
+    def get_eth(self) -> Optional[MinerFeesItem]:
         """
         Get method for the eth
         :return: eth
         """
         return self.__eth
 
-    def set_eth(self, eth: MinerFeesItem):
+    def set_eth(self, eth: MinerFeesItem) -> None:
         """
         Set method for the eth
         :param eth: eth
         """
         self.__eth = eth
 
-    def get_usdc(self):
+    def get_usdc(self) -> Optional[MinerFeesItem]:
         """
         Get method for the usdc
         :return: usdc
         """
         return self.__usdc
 
-    def set_usdc(self, usdc: MinerFeesItem):
+    def set_usdc(self, usdc: MinerFeesItem) -> None:
         """
         Set method for the usdc
         :param usdc: usdc
         """
         self.__usdc = usdc
 
-    def get_gusd(self):
+    def get_gusd(self) -> Optional[MinerFeesItem]:
         """
         Get method for the gusd
         :return: gusd
         """
         return self.__gusd
 
-    def set_gusd(self, gusd: MinerFeesItem):
+    def set_gusd(self, gusd: MinerFeesItem) -> None:
         """
         Set method for the gusd
         :param gusd: gusd
         """
         self.__gusd = gusd
 
-    def get_doge(self):
+    def get_doge(self) -> Optional[MinerFeesItem]:
         """
         Get method for the doge
         :return: doge
         """
         return self.__doge
 
-    def set_doge(self, doge: MinerFeesItem):
+    def set_doge(self, doge: MinerFeesItem) -> None:
         """
         Set method for the doge
         :param doge: doge
         """
         self.__doge = doge
 
-    def get_ltc(self):
+    def get_ltc(self) -> Optional[MinerFeesItem]:
         """
         Get method for the ltc
         :return: ltc
         """
         return self.__ltc
 
-    def set_ltc(self, ltc: MinerFeesItem):
+    def set_ltc(self, ltc: MinerFeesItem) -> None:
         """
         Set method for the ltc
         :param ltc: ltc
         """
         self.__ltc = ltc
 
-    def get_pax(self):
+    def get_pax(self) -> Optional[MinerFeesItem]:
         """
         Get method for the pax
         :return: pax
         """
         return self.__pax
 
-    def set_pax(self, pax: MinerFeesItem):
+    def set_pax(self, pax: MinerFeesItem) -> None:
         """
         Set method for the pax
         :param pax: pax
         """
         self.__pax = pax
 
-    def get_busd(self):
+    def get_busd(self) -> Optional[MinerFeesItem]:
         """
         Get method for the busd
         :return: busd
         """
         return self.__busd
 
-    def set_busd(self, busd: MinerFeesItem):
+    def set_busd(self, busd: MinerFeesItem) -> None:
         """
         Set method for the busd
         :param busd: busd
         """
         self.__busd = busd
 
-    def get_xrp(self):
+    def get_xrp(self) -> Optional[MinerFeesItem]:
         """
         Get method for the xrp
         :return: xrp
         """
         return self.__xrp
 
-    def set_xrp(self, xrp: MinerFeesItem):
+    def set_xrp(self, xrp: MinerFeesItem) -> None:
         """
         Set method for the xrp
         :param xrp: xrp
         """
         self.__xrp = xrp
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "btc": self.get_btc(),
-            "bch": self.get_bch(),
-            "eth": self.get_eth(),
-            "usdc": self.get_usdc(),
-            "gusd": self.get_gusd(),
-            "pax": self.get_pax(),
-            "doge": self.get_doge(),
-            "ltc": self.get_ltc(),
-            "xrp": self.get_xrp(),
-            "busd": self.get_busd(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/invoice/refund_info.py` & `bitpay-4.0.0/src/bitpay/models/invoice/refund_info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 """
 RefundInfo
 """
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional, List
+
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class RefundInfo:
     """
     Information about refund
     """
 
     __support_request = None
     __currency = None
-    __amounts = None
+    __amounts: Optional[List[dict]] = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
+                value = ModelUtil.get_field_value(key, value, {}, {"amounts": "dict"})
+
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_support_request(self):
+    def get_support_request(self) -> Optional[str]:
         """
         Get method for the support_request
         :return: support_request
         """
         return self.__support_request
 
-    def set_support_request(self, support_request):
+    def set_support_request(self, support_request: Optional[str]) -> None:
         """
         Set method for the support_request
         :param support_request: support_request
         """
         self.__support_request = support_request
 
-    def get_currency(self):
+    def get_currency(self) -> Optional[str]:
         """
         Get method for the currency
         :return: currency
         """
         return self.__currency
 
-    def set_currency(self, currency):
+    def set_currency(self, currency: Optional[str]) -> None:
         """
         Set method for the currency
         :param currency: currency
         """
         self.__currency = currency
 
-    def get_amounts(self):
+    def get_amounts(self) -> Optional[List[dict]]:
         """
         Get method for the amounts
         :return: amounts
         """
         return self.__amounts
 
-    def set_amounts(self, amounts):
+    def set_amounts(self, amounts: Optional[List[dict]]) -> None:
         """
         Set method for the amounts
         :param amounts: amounts
         """
         self.__amounts = amounts
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "supportRequest": self.get_support_request(),
-            "currency": self.get_currency(),
-            "amounts": self.get_amounts(),
-        }
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/invoice/universal_codes.py` & `bitpay-4.0.0/src/bitpay/models/invoice/universal_codes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 """
 UniversalCodes
 """
-from ...utils import key_utils
+from typing import Optional
+
+from bitpay.utils import key_utils
+from bitpay.utils.model_util import ModelUtil
 
 
 class UniversalCodes:
     """
     object containing wallet-specific URLs for payment protocol
     """
 
     __payment_string = None
     __verification_link = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
                 getattr(
                     self, "set_%s" % key_utils.change_camel_case_to_snake_case(key)
                 )(value)
             except AttributeError:
                 pass
 
-    def get_payment_string(self):
+    def get_payment_string(self) -> Optional[str]:
         """
         Get method for to payment_string
         :return: payment_string
         """
         return self.__payment_string
 
-    def set_payment_string(self, payment_string):
+    def set_payment_string(self, payment_string: Optional[str]) -> None:
         """
         Set method for to payment_string
         :param payment_string: payment_string
         """
         self.__payment_string = payment_string
 
-    def get_verification_link(self):
+    def get_verification_link(self) -> Optional[str]:
         """
         Get method for to enabled
         :return: enabled
         """
         return self.__verification_link
 
-    def set_verification_link(self, verification_link):
+    def set_verification_link(self, verification_link: Optional[str]) -> None:
         """
         Set method for to verification_link
         :param verification_link: verification_link
         """
         self.__verification_link = verification_link
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "paymentString": self.get_payment_string(),
-            "verificationLink": self.get_verification_link(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/invoice/invoice.py` & `bitpay-4.0.0/src/bitpay/models/invoice/invoice.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1094 +1,1064 @@
 """
 Invoice
 """
+from typing import Union, List, Optional, Dict
+
 from .buyer import Buyer
 from .shopper import Shopper
 from .miner_fees import MinerFees
 from .refund_info import RefundInfo
+from .transaction import Transaction
 from .universal_codes import UniversalCodes
 from .itemized_details import ItemizedDetails
 from .buyer_provided_info import BuyerProvidedInfo
-from ...utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
 from .supported_transaction_currencies import SupportedTransactionCurrencies
+from bitpay.utils.model_util import ModelUtil
 
 
 class Invoice:
     """
     Invoices are time-sensitive payment requests addressed to specific buyers.
     An invoice has a fixed price,typically denominated in fiat currency.
     It also has an equivalent price in the supported cryptocurrencies,
     calculated by BitPay, at a locked exchange rate with an expiration
     time of 15 minutes.
     """
 
-    __currency = ""
+    __currency = None
 
-    __guid = ""
-    __token = ""
+    __guid = None
+    __token = None
 
     __price = None
     __pos_data = None
-    __notification_url = ""
-    __transaction_speed = ""
+    __notification_url = None
+    __transaction_speed = None
     __full_notifications = False
-    __notification_email = ""
-    __redirect_URL = ""
-    __order_id = ""
-    __item_desc = ""
-    __item_code = ""
+    __notification_email = None
+    __redirect_URL = None
+    __order_id = None
+    __item_desc = None
+    __item_code = None
     __physical = False
-    __payment_currencies = []
-    __payment_subtotals = None
-    __payment_totals = None
-    __payment_display_totals = None
-    __payment_display_subtotals = None
-    __payment_codes = None
+    __payment_currencies: Optional[List[str]] = None
+    __payment_subtotals: Optional[dict] = None
+    __payment_totals: Optional[dict] = None
+    __payment_display_totals: Optional[dict] = None
+    __payment_display_subtotals: Optional[dict] = None
+    __payment_codes: Optional[dict] = None
     __acceptance_window = None
-    __buyer = Buyer()
-    __refund_addresses = None
-    __close_url = ""
+    __buyer = None
+    __refund_addresses: Optional[List[str]]
+    __close_url = None
     __auto_redirect = False
-    __json_paypro_required = None
+    __json_paypro_required = False
 
     __id = None
     __url = None
     __status = None
-    __low_fee_detected = None
+    __low_fee_detected = False
     __invoice_time = None
     __expiration_time = None
     __current_time = None
-    __transactions = None
+    __transactions: Optional[List[Transaction]] = None
     __exception_status = None
     __target_confirmations = None
-    __refund_address_request_pending = None
+    __refund_address_request_pending = False
     __buyer_provided_email = None
-    __buyer_provided_info = BuyerProvidedInfo()
-    __supported_transaction_currencies = SupportedTransactionCurrencies()
-    __miner_fees = MinerFees()
-    __non_paypro_payment_received = None
-    __shopper = Shopper()
+    __buyer_provided_info = None
+    __buyer_sms = None
+    __supported_transaction_currencies = None
+    __miner_fees = None
+    __non_pay_pro_payment_received = False
+    __shopper = None
     __bill_id = None
-    __refund_info = RefundInfo()
+    __refund_info: Optional[List[RefundInfo]] = None
     __extended_notifications = False
+    __invoice_buyer_provided_info = None
 
     __transaction_currency = None
     __underpaid_amount = None
     __overpaid_amount = None
     __amount_paid = None
     __display_amount_paid = None
-    __exchange_rates = None
+    __exchange_rates: Optional[dict] = None
 
     __payment_string = None
     __verification_link = None
     __buyer_email = None
-    __declined_amount = None
     __merchant_name = None
     __forced_buyer_selected_wallet = None
     __forced_buyer_selected_transaction_currency = None
-    __itemized_details = ItemizedDetails()
-    __universal_codes = UniversalCodes()
-    __is_cancelled = None
-    __bitpay_id_required = None
-    __rate_refresh_time = None
-
-    def __init__(self, price=None, currency=None, **kwargs):
+    __itemized_details: Optional[List[ItemizedDetails]] = None
+    __universal_codes = None
+    __is_cancelled = False
+    __bitpay_id_required = False
+
+    def __init__(
+        self,
+        price: Optional[float] = None,
+        currency: Optional[str] = None,
+        **kwargs: dict
+    ) -> None:
         self.set_price(price)
         self.set_currency(currency)
 
         for key, value in kwargs.items():
             try:
-                if key in [
-                    "buyer",
-                    "buyerProvidedInfo",
-                    "shopper",
-                    "supportedTransactionCurrencies",
-                    "minerFees",
-                    "refundInfo",
-                    "universalCodes",
-                    "itemizedDetails",
-                ]:
-                    klass = globals()[key[0].upper() + key[1:]]
-
-                    if isinstance(value, list):
-                        objs = []
-                        for obj in value:
-                            objs.append(klass(**obj))
-                        value = objs
-                    else:
-                        value = klass(**value)
+                value = ModelUtil.get_field_value(
+                    key,
+                    value,
+                    {
+                        "price": "float",
+                        "amountPaid": "float",
+                        "underpaidAmount": "float",
+                        "overpaidAmount": "float",
+                        "physical": "bool",
+                        "autoRedirect": "bool",
+                        "acceptanceWindow": "int",
+                        "lowFeeDetected": "bool",
+                        "refundAddressRequestPending": "bool",
+                        "extendedNotifications": "bool",
+                        "isCancelled": "bool",
+                        "bitpayIdRequired": "bool",
+                        "nonPayProPaymentReceived": "bool",
+                        "jsonPayProRequired": "bool",
+                        "invoiceTime": "int",
+                        "expirationTime": "int",
+                        "currentTime": "int",
+                        "targetConfirmations": "int",
+                        "buyer": Buyer,
+                        "buyerProvidedInfo": BuyerProvidedInfo,
+                        "shopper": Shopper,
+                        "supportedTransactionCurrencies": SupportedTransactionCurrencies,
+                        "minerFees": MinerFees,
+                        "universalCodes": UniversalCodes,
+                        "fullNotifications": "bool",
+                    },
+                    {
+                        "paymentCurrencies": "str",
+                        "paymentSubtotals": "dict",
+                        "paymentTotals": "dict",
+                        "paymentDisplayTotals": "dict",
+                        "paymentDisplaySubTotals": "dict",
+                        "refundAddresses": "str",
+                        "itemizedDetails": ItemizedDetails,
+                        "refundInfo": RefundInfo,
+                        "paymentCodes": "dict",
+                        "transactions": Transaction,
+                        "exchangeRates": "dict",
+                    },
+                )
+
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_guid(self):
+    def get_guid(self) -> Optional[str]:
         """
         Get method for the guid
         :return: guid
         """
         return self.__guid
 
-    def set_guid(self, guid):
+    def set_guid(self, guid: Optional[str]) -> None:
         """
         Set method for the guid
         :param guid: guid
         """
         self.__guid = guid
 
-    def get_token(self):
+    def get_token(self) -> Optional[str]:
         """
         Get method for the token
         :return: token
         """
         return self.__token
 
-    def set_token(self, token):
+    def set_token(self, token: Optional[str]) -> None:
         """
         Set method for the token
         :param token: token
         """
         self.__token = token
 
-    def get_declined_amount(self):
-        """
-        Get method for the declined_amount
-        :return: declined_amount
-        """
-        return self.__declined_amount
-
-    def set_declined_amount(self, declined_amount):
-        """
-        Set method for the declined_amount
-        :param declined_amount: declined_amount
-        """
-        self.__declined_amount = declined_amount
-
-    def get_pos_data(self):
+    def get_pos_data(self) -> Optional[str]:
         """
         Get method for the pos_data
         :return: pos_data
         """
         return self.__pos_data
 
-    def set_pos_data(self, pos_data):
+    def set_pos_data(self, pos_data: Optional[str]) -> None:
         """
         Set method for the pos_data
         :param pos_data: posData
         """
         self.__pos_data = pos_data
 
-    def get_notification_url(self):
+    def get_notification_url(self) -> Optional[str]:
         """
         Get method for the notification_url
         :return: notification_url
         """
         return self.__notification_url
 
-    def set_notification_url(self, notification_url):
+    def set_notification_url(self, notification_url: Optional[str]) -> None:
         """
         Set method for the notification_url
         :param notification_url: notification_url
         """
         self.__notification_url = notification_url
 
-    def get_transaction_speed(self):
+    def get_transaction_speed(self) -> Optional[str]:
         """
         Get method for the transaction_speed
         :return: transaction_speed
         """
         return self.__transaction_speed
 
-    def set_transaction_speed(self, transaction_speed):
+    def set_transaction_speed(self, transaction_speed: Optional[str]) -> None:
         """
         Set method for the transaction_speed
         :param transaction_speed: transaction_speed
         """
         self.__transaction_speed = transaction_speed
 
-    def get_full_notifications(self):
+    def get_full_notifications(self) -> bool:
         """
         Get method for the full_notifications
         :return: full_notifications
         """
         return self.__full_notifications
 
-    def set_full_notifications(self, full_notifications):
+    def set_full_notifications(self, full_notifications: bool) -> None:
         """
         Set method for the full_notifications
         :param full_notifications: full_notifications
         """
         self.__full_notifications = full_notifications
 
-    def get_notification_email(self):
+    def get_notification_email(self) -> Optional[str]:
         """
         Get method for the notification_email
         :return: notification_email
         """
         return self.__notification_email
 
-    def set_notification_email(self, notification_email):
+    def set_notification_email(self, notification_email: Optional[str]) -> None:
         """
         Set method for the notification_email
         :param notification_email: notification_email
         """
         self.__notification_email = notification_email
 
-    def get_redirect_u_r_l(self):
+    def get_redirect_u_r_l(self) -> Optional[str]:
         """
         Get method for the redirect_URL
         :return: redirect_URL
         """
         return self.__redirect_URL
 
-    def set_redirect_u_r_l(self, redirect_URL):
+    def set_redirect_u_r_l(self, redirect_url: Optional[str]) -> None:
         """
         Set method for the redirect_URL
-        :param redirect_URL: redirect_URL
+        :param redirect_url: redirect_URL
         """
-        self.__redirect_URL = redirect_URL
+        self.__redirect_URL = redirect_url
 
-    def get_order_id(self):
+    def get_order_id(self) -> Optional[str]:
         """
         Get method for the order_id
         :return: order_id
         """
         return self.__order_id
 
-    def set_order_id(self, order_id):
+    def set_order_id(self, order_id: Optional[str]) -> None:
         """
         Set method for the order_id
         :param order_id: order_id
         """
         self.__order_id = order_id
 
-    def get_item_desc(self):
+    def get_item_desc(self) -> Optional[str]:
         """
         Get method for the item_desc
         :return: item_desc
         """
         return self.__item_desc
 
-    def set_item_desc(self, item_desc):
+    def set_item_desc(self, item_desc: Optional[str]) -> None:
         """
         Set method for the item_desc
         :param item_desc: item_desc
         """
         self.__item_desc = item_desc
 
-    def get_item_code(self):
+    def get_item_code(self) -> Optional[str]:
         """
         Get method for the item_code
         :return: item_code
         """
         return self.__item_code
 
-    def set_item_code(self, item_code):
+    def set_item_code(self, item_code: Optional[str]) -> None:
         """
         Set method for the item_code
         :param item_code: item_code
         """
         self.__item_code = item_code
 
-    def get_physical(self):
+    def get_physical(self) -> bool:
         """
         Get method for the physical
         :return: physical
         """
         return self.__physical
 
-    def set_physical(self, physical):
+    def set_physical(self, physical: bool) -> None:
         """
         Set method for the physical
         :param physical: physical
         """
         self.__physical = physical
 
-    def get_payment_currencies(self):
+    def get_payment_currencies(self) -> Optional[List[str]]:
         """
         Get method for the payment_currencies
         :return: payment_currencies
         """
         return self.__payment_currencies
 
-    def set_payment_currencies(self, payment_currencies):
+    def set_payment_currencies(self, payment_currencies: List[str]) -> None:
         """
         Set method for the payment_currencies
         :param payment_currencies: payment_currencies
         """
         self.__payment_currencies = payment_currencies
 
-    def get_payment_subtotals(self):
+    def get_payment_subtotals(self) -> Optional[dict]:
         """
         Get method for the payment_subtotals
         :return: payment_subtotals
         """
         return self.__payment_subtotals
 
-    def set_payment_subtotals(self, payment_subtotals):
+    def set_payment_subtotals(self, payment_subtotals: Optional[dict]) -> None:
         """
         Set method for the payment_subtotals
         :param payment_subtotals: payment_subtotals
         """
         self.__payment_subtotals = payment_subtotals
 
-    def get_payment_totals(self):
+    def get_payment_totals(self) -> Optional[dict]:
         """
         Get method for the payment_totals
         :return: payment_totals
         """
         return self.__payment_totals
 
-    def set_payment_totals(self, payment_totals):
+    def set_payment_totals(self, payment_totals: Optional[dict]) -> None:
         """
         Set method for the payment_totals
         :param payment_totals: payment_totals
         """
         self.__payment_totals = payment_totals
 
-    def get_payment_display_totals(self):
+    def get_payment_display_totals(self) -> Optional[dict]:
         """
         Get method for the payment_display_totals
         :return: payment_display_totals
         """
         return self.__payment_display_totals
 
-    def set_payment_display_totals(self, payment_display_totals):
+    def set_payment_display_totals(
+        self, payment_display_totals: Optional[dict]
+    ) -> None:
         """
         Set method for the payment_display_totals
         :param payment_display_totals: payment_display_totals
         """
         self.__payment_display_totals = payment_display_totals
 
-    def get_payment_display_sub_totals(self):
+    def get_payment_display_sub_totals(self) -> Optional[dict]:
         """
         Get method for the payment_display_subtotals
         :return: payment_display_subtotals
         """
         return self.__payment_display_subtotals
 
-    def set_payment_display_sub_totals(self, payment_display_subtotals):
+    def set_payment_display_sub_totals(
+        self, payment_display_subtotals: Optional[dict]
+    ) -> None:
         """
         Set method for the payment_display_subtotals
         :param payment_display_subtotals: payment_display_subtotals
         """
         self.__payment_display_subtotals = payment_display_subtotals
 
-    def get_payment_codes(self):
+    def get_payment_codes(self) -> Optional[dict]:
         """
         Get method for the payment_codes
         :return: payment_codes
         """
         return self.__payment_codes
 
-    def set_payment_codes(self, payment_codes):
+    def set_payment_codes(self, payment_codes: Optional[dict]) -> None:
         """
         Set method for the payment_codes
         :param payment_codes: payment_codes
         """
         self.__payment_codes = payment_codes
 
-    def get_acceptance_window(self):
+    def get_acceptance_window(self) -> Optional[int]:
         """
         Get method for the acceptance_window
         :return: acceptance_window
         """
         return self.__acceptance_window
 
-    def set_acceptance_window(self, acceptance_window):
+    def set_acceptance_window(self, acceptance_window: Optional[int]) -> None:
         """
         Set method for the acceptance_window
         :param acceptance_window: acceptance_window
         """
         self.__acceptance_window = acceptance_window
 
-    def get_refund_addresses(self):
+    def get_refund_addresses(self) -> Optional[List[str]]:
         """
         Get method for the refund_addresses
         :return: refund_addresses
         """
         return self.__refund_addresses
 
-    def set_refund_addresses(self, refund_addresses):
+    def set_refund_addresses(self, refund_addresses: Optional[List[str]]) -> None:
         """
         Set method for the refund_addresses
         :param refund_addresses: refund_addresses
         """
         self.__refund_addresses = refund_addresses
 
-    def get_close_url(self):
+    def get_close_url(self) -> Optional[str]:
         """
         Get method for the close_url
         :return: close_url
         """
         return self.__close_url
 
-    def set_close_url(self, close_url):
+    def set_close_url(self, close_url: Optional[str]) -> None:
         """
         Set method for the close_url
         :param close_url: close_url
         """
         self.__close_url = close_url
 
-    def get_auto_redirect(self):
+    def get_auto_redirect(self) -> bool:
         """
         Get method for the auto_redirect
         :return: auto_redirect
         """
         return self.__auto_redirect
 
-    def set_auto_redirect(self, auto_redirect):
+    def set_auto_redirect(self, auto_redirect: bool) -> None:
         """
         Set method for the auto_redirect
         :param auto_redirect: auto_redirect
         """
         self.__auto_redirect = auto_redirect
 
-    def get_json_pay_pro_required(self):
+    def get_json_pay_pro_required(self) -> bool:
         """
         Get method for the json_paypro_required
         :return: json_paypro_required
         """
         return self.__json_paypro_required
 
-    def set_json_pay_pro_required(self, json_paypro_required):
+    def set_json_pay_pro_required(self, json_paypro_required: bool) -> None:
         """
         Set method for the json_paypro_required
         :param json_paypro_required: json_paypro_required
         """
         self.__json_paypro_required = json_paypro_required
 
-    def get_id(self):
+    def get_id(self) -> Optional[str]:
         """
         Get method for the id
         :return: id
         """
         return self.__id
 
-    def set_id(self, id):
+    def set_id(self, id: Optional[str]) -> None:
         """
         Set method for the id
         :param id: id
         """
         self.__id = id
 
-    def get_url(self):
+    def get_url(self) -> Optional[str]:
         """
         Get method for the url
         :return: url
         """
         return self.__url
 
-    def set_url(self, url):
+    def set_url(self, url: Optional[str]) -> None:
         """
         Set method for the url
         :param url: url
         """
         self.__url = url
 
-    def get_status(self):
+    def get_status(self) -> Optional[str]:
         """
         Get method for the status
         :return: status
         """
         return self.__status
 
-    def set_status(self, status):
+    def set_status(self, status: Optional[str]) -> None:
         """
         Set method for the status
         :param status: status
         """
         self.__status = status
 
-    def get_low_fee_detected(self):
+    def get_low_fee_detected(self) -> bool:
         """
         Get method for the low_fee_detected
         :return: low_fee_detected
         """
         return self.__low_fee_detected
 
-    def set_low_fee_detected(self, low_fee_detected):
+    def set_low_fee_detected(self, low_fee_detected: bool) -> None:
         """
         Set method for the low_fee_detected
         :param low_fee_detected: low_fee_detected
         """
         self.__low_fee_detected = low_fee_detected
 
-    def get_invoice_time(self):
+    def get_invoice_time(self) -> Optional[int]:
         """
         Get method for the invoice_time
         :return: invoice_time
         """
         return self.__invoice_time
 
-    def set_invoice_time(self, invoice_time):
+    def set_invoice_time(self, invoice_time: Optional[int]) -> None:
         """
         Set method for the invoice_time
         :param invoice_time: invoice_time
         """
         self.__invoice_time = invoice_time
 
-    def get_expiration_time(self):
+    def get_expiration_time(self) -> Optional[int]:
         """
         Get method for the expiration_time
         :return: expiration_time
         """
         return self.__expiration_time
 
-    def set_expiration_time(self, expiration_time):
+    def set_expiration_time(self, expiration_time: Optional[int]) -> None:
         """
         Set method for the expiration_time
         :param expiration_time: expiration_time
         """
         self.__expiration_time = expiration_time
 
-    def get_current_time(self):
+    def get_current_time(self) -> Optional[int]:
         """
         Get method for the current_time
         :return: current_time
         """
         return self.__current_time
 
-    def set_current_time(self, current_time):
+    def set_current_time(self, current_time: Optional[int]) -> None:
         """
         Set method for the current_time
         :param current_time: current_time
         """
         self.__current_time = current_time
 
-    def get_transactions(self):
+    def get_transactions(self) -> Optional[List[Transaction]]:
         """
         Get method for the transactions
         :return: transactions
         """
         return self.__transactions
 
-    def set_transactions(self, transactions):
+    def set_transactions(self, transactions: List[Transaction]) -> None:
         """
         Set method for the transactions
         :param transactions: transactions
         """
         self.__transactions = transactions
 
-    def get_exception_status(self):
+    def get_exception_status(self) -> Optional[str]:
         """
         Get method for the exception_status
         :return: exception_status
         """
         return self.__exception_status
 
-    def set_exception_status(self, exception_status):
+    def set_exception_status(self, exception_status: Optional[str]) -> None:
         """
         Set method for the exception_status
         :param exception_status: exception_status
         """
         self.__exception_status = exception_status
 
-    def get_target_confirmations(self):
+    def get_target_confirmations(self) -> Optional[int]:
         """
         Get method for the target_confirmations
         :return: target_confirmations
         """
         return self.__target_confirmations
 
-    def set_target_confirmations(self, target_confirmations):
+    def set_target_confirmations(self, target_confirmations: Optional[int]) -> None:
         """
         Set method for the target_confirmations
         :param target_confirmations: target_confirmations
         """
         self.__target_confirmations = target_confirmations
 
-    def get_refund_address_request_pending(self):
+    def get_refund_address_request_pending(self) -> bool:
         """
         Get method for the refund_address_request_pending
         :return: refund_address_request_pending
         """
         return self.__refund_address_request_pending
 
-    def set_refund_address_request_pending(self, refund_address_request_pending):
+    def set_refund_address_request_pending(
+        self, refund_address_request_pending: bool
+    ) -> None:
         """
         Set method for the refund_address_request_pending
         :param refund_address_request_pending: refund_address_request_pending
         """
         self.__refund_address_request_pending = refund_address_request_pending
 
-    def get_buyer_provided_email(self):
+    def get_buyer_provided_email(self) -> Optional[str]:
         """
         Get method for the buyer_provided_email
         :return: buyer_provided_email
         """
         return self.__buyer_provided_email
 
-    def set_buyer_provided_email(self, buyer_provided_email):
+    def set_buyer_provided_email(self, buyer_provided_email: Optional[str]) -> None:
         """
         Set method for the buyer_provided_email
         :param buyer_provided_email: buyer_provided_email
         """
         self.__buyer_provided_email = buyer_provided_email
 
-    def get_buyer_provided_info(self):
+    def get_buyer_provided_info(self) -> Optional[BuyerProvidedInfo]:
         """
         Get method for the buyer_provided_info
         :return: buyer_provided_info
         """
         return self.__buyer_provided_info
 
-    def set_buyer_provided_info(self, buyer_provided_info: BuyerProvidedInfo):
+    def set_buyer_provided_info(self, buyer_provided_info: BuyerProvidedInfo) -> None:
         """
         Set method for the buyer_provided_info
         :param buyer_provided_info: buyer_provided_info
         """
         self.__buyer_provided_info = buyer_provided_info
 
-    def get_supported_transaction_currencies(self):
+    def get_supported_transaction_currencies(
+        self,
+    ) -> Optional[SupportedTransactionCurrencies]:
         """
         Get method for the supported_transaction_currencies
         :return: supported_transaction_currencies
         """
         return self.__supported_transaction_currencies
 
     def set_supported_transaction_currencies(
         self, supported_transaction_currencies: SupportedTransactionCurrencies
-    ):
+    ) -> None:
         """
         Set method for the supported_transaction_currencies
         :param supported_transaction_currencies: supported_transaction_currencies
         """
         self.__supported_transaction_currencies = supported_transaction_currencies
 
-    def get_miner_fees(self):
+    def get_miner_fees(self) -> Optional[MinerFees]:
         """
         Get method for the miner_fees
         :return: miner_fees
         """
         return self.__miner_fees
 
-    def set_miner_fees(self, miner_fees: MinerFees):
+    def set_miner_fees(self, miner_fees: Optional[MinerFees]) -> None:
         """
         Set method for the miner_fees
         :param miner_fees: miner_fees
         """
         self.__miner_fees = miner_fees
 
-    def get_non_paypro_payment_received(self):
+    def get_non_pay_pro_payment_received(self) -> bool:
         """
         Get method for the non_paypro_payment_received
         :return: non_paypro_payment_received
         """
-        return self.__non_paypro_payment_received
+        return self.__non_pay_pro_payment_received
 
-    def set_non_paypro_payment_received(self, non_paypro_payment_received):
+    def set_non_pay_pro_payment_received(
+        self, non_pay_pro_payment_received: bool
+    ) -> None:
         """
         Set method for the non_paypro_payment_received
-        :param non_paypro_payment_received: non_paypro_payment_received
+        :param non_pay_pro_payment_received: non_paypro_payment_received
         """
-        self.__non_paypro_payment_received = non_paypro_payment_received
+        self.__non_pay_pro_payment_received = non_pay_pro_payment_received
 
-    def get_shopper(self):
+    def get_shopper(self) -> Optional[Shopper]:
         """
         Get method for the shopper
         :return: shopper
         """
         return self.__shopper
 
-    def set_shopper(self, shopper: Shopper):
+    def set_shopper(self, shopper: Optional[Shopper]) -> None:
         """
         Set method for the shopper
         :param shopper: shopper
         """
         self.__shopper = shopper
 
-    def get_bill_id(self):
+    def get_bill_id(self) -> Optional[str]:
         """
         Get method for the bill_id
         :return: bill_id
         """
         return self.__bill_id
 
-    def set_bill_id(self, bill_id):
+    def set_bill_id(self, bill_id: Optional[str]) -> None:
         """
         Set method for the bill_id
         :param bill_id: bill_id
         """
         self.__bill_id = bill_id
 
-    def get_refund_info(self):
+    def get_refund_info(self) -> Optional[List[RefundInfo]]:
         """
         Get method for the refund_info
         :return: refund_info
         """
         return self.__refund_info
 
-    def set_refund_info(self, refund_info: RefundInfo):
+    def set_refund_info(self, refund_info: Optional[List[RefundInfo]]) -> None:
         """
         Set method for the refund_info
         :param refund_info: refund_info
         """
         self.__refund_info = refund_info
 
-    def get_extended_notifications(self):
+    def get_extended_notifications(self) -> bool:
         """
         Get method for the extended_notifications
         :return: extended_notifications
         """
         return self.__extended_notifications
 
-    def set_extended_notifications(self, extended_notifications):
+    def set_extended_notifications(self, extended_notifications: bool) -> None:
         """
         Set method for the extended_notifications
         :param extended_notifications: extended_notifications
         """
         self.__extended_notifications = extended_notifications
 
-    def get_transaction_currency(self):
+    def get_transaction_currency(self) -> Optional[str]:
         """
         Get method for the transaction_currency
         :return: transaction_currency
         """
         return self.__transaction_currency
 
-    def set_transaction_currency(self, transaction_currency):
+    def set_transaction_currency(self, transaction_currency: Optional[str]) -> None:
         """
         Set method for the transaction_currency
         :param transaction_currency: transaction_currency
         """
         self.__transaction_currency = transaction_currency
 
-    def get_underpaid_amount(self):
+    def get_underpaid_amount(self) -> Optional[str]:
         """
         Get method for the underpaid_amount
         :return: underpaid_amount
         """
         return self.__underpaid_amount
 
-    def set_underpaid_amount(self, underpaid_amount):
+    def set_underpaid_amount(self, underpaid_amount: Optional[float]) -> None:
         """
         Set method for the underpaid_amount
         :param underpaid_amount: underpaid_amount
         """
         self.__underpaid_amount = underpaid_amount
 
-    def get_overpaid_amount(self):
+    def get_overpaid_amount(self) -> Optional[float]:
         """
         Get method for the overpaid_amount
         :return: overpaid_amount
         """
         return self.__overpaid_amount
 
-    def set_overpaid_amount(self, overpaid_amount):
+    def set_overpaid_amount(self, overpaid_amount: Optional[float]) -> None:
         """
         Set method for the overpaid_amount
         :param overpaid_amount: overpaid_amount
         """
         self.__overpaid_amount = overpaid_amount
 
-    def get_amount_paid(self):
+    def get_amount_paid(self) -> Optional[float]:
         """
         Get method for the amount_paid
         :return: overpaid_amount
         """
         return self.__amount_paid
 
-    def set_amount_paid(self, amount_paid):
+    def set_amount_paid(self, amount_paid: Optional[float]) -> None:
         """
         Set method for the amount_paid
         :param amount_paid: amount_paid
         """
         self.__amount_paid = amount_paid
 
-    def get_display_amount_paid(self):
+    def get_display_amount_paid(self) -> Optional[str]:
         """
         Get method for the display_amount_paid
         :return: display_amount_paid
         """
         return self.__display_amount_paid
 
-    def set_display_amount_paid(self, display_amount_paid):
+    def set_display_amount_paid(self, display_amount_paid: Optional[str]) -> None:
         """
         Set method for the display_amount_paid
         :param display_amount_paid: display_amount_paid
         """
         self.__display_amount_paid = display_amount_paid
 
-    def get_exchange_rates(self):
+    def get_exchange_rates(self) -> Optional[dict]:
         """
         Get method for the exchange_rates
         :return: exchange_rates
         """
         return self.__exchange_rates
 
-    def set_exchange_rates(self, exchange_rates):
+    def set_exchange_rates(self, exchange_rates: Optional[dict]) -> None:
         """
         Set method for the exchange_rates
         :param exchange_rates: exchange_rates
         """
         self.__exchange_rates = exchange_rates
 
-    def get_price(self):
+    def get_price(self) -> Optional[float]:
         """
         Get method for the price
         :return: price
         """
         return self.__price
 
-    def set_price(self, price):
+    def set_price(self, price: Optional[float]) -> None:
         """
         Set method for the price
         :param price: price
         """
         self.__price = price
 
-    def get_currency(self):
+    def get_currency(self) -> Optional[str]:
         """
         Get method for the currency
         :return: currency
         """
         return self.__currency
 
-    def set_currency(self, currency):
+    def set_currency(self, currency: Optional[str]) -> None:
         """
         Set method for the currency
         :param currency: currency
         """
         self.__currency = currency
 
-    def get_payment_string(self):
+    def get_payment_string(self) -> Optional[str]:
         """
         Get method for the payment_string
         :return: payment_string
         """
         return self.__payment_string
 
-    def set_payment_string(self, payment_string):
+    def set_payment_string(self, payment_string: Optional[str]) -> None:
         """
         Set method for the payment_string
         :param payment_string: payment_string
         """
         self.__payment_string = payment_string
 
-    def get_verification_link(self):
+    def get_verification_link(self) -> Optional[str]:
         """
         Get method for the verification_link
         :return: verification_link
         """
         return self.__verification_link
 
-    def set_verification_link(self, verification_link):
+    def set_verification_link(self, verification_link: Optional[str]) -> None:
         """
         Set method for the verification_link
         :param verification_link: verification_link
         """
         self.__verification_link = verification_link
 
-    def get_buyer_email(self):
+    def get_buyer_email(self) -> Optional[str]:
         """
         Get method for the buyer_email
         :return: buyer_email
         """
         return self.__buyer_email
 
-    def set_buyer_email(self, buyer_email):
+    def set_buyer_email(self, buyer_email: Optional[str]) -> None:
         """
         Set method for the buyer_email
         :param buyer_email: buyer_email
         """
         self.__buyer_email = buyer_email
 
-    def get_merchant_name(self):
+    def get_merchant_name(self) -> Optional[str]:
         """
         Get method for the merchant_name
         :return: merchant_name
         """
         return self.__merchant_name
 
-    def set_merchant_name(self, merchant_name):
+    def set_merchant_name(self, merchant_name: Optional[str]) -> None:
         """
         Set method for the merchant_name
         :param merchant_name: merchant_name
         """
         self.__merchant_name = merchant_name
 
-    def get_forced_buyer_selected_wallet(self):
+    def get_forced_buyer_selected_wallet(self) -> Optional[str]:
         """
         Get method for the forced_buyer_selected_wallet
         :return: forced_buyer_selected_wallet
         """
         return self.__forced_buyer_selected_wallet
 
-    def set_forced_buyer_selected_wallet(self, forced_buyer_selected_wallet):
+    def set_forced_buyer_selected_wallet(
+        self, forced_buyer_selected_wallet: Optional[str]
+    ) -> None:
         """
         Set method for the forced_buyer_selected_wallet
         :param forced_buyer_selected_wallet: forced_buyer_selected_wallet
         """
         self.__forced_buyer_selected_wallet = forced_buyer_selected_wallet
 
-    def get_forced_buyer_selected_transaction_currency(self):
+    def get_forced_buyer_selected_transaction_currency(self) -> Optional[str]:
         """
         Get method for the forced_buyer_selected_transaction_currency
         :return: forced_buyer_selected_transaction_currency
         """
         return self.__forced_buyer_selected_transaction_currency
 
     def set_forced_buyer_selected_transaction_currency(
-        self, forced_buyer_selected_transaction_currency
-    ):
+        self, forced_buyer_selected_transaction_currency: Optional[str]
+    ) -> None:
         """
         Set method for the forced_buyer_selected_transaction_currency
         :param forced_buyer_selected_transaction_currency: forced_buyer_selected_transaction_currency
         """
         self.__forced_buyer_selected_transaction_currency = (
             forced_buyer_selected_transaction_currency
         )
 
-    def get_is_cancelled(self):
+    def get_is_cancelled(self) -> bool:
         """
         Get method for the is_cancelled
         :return: is_cancelled
         """
         return self.__is_cancelled
 
-    def set_is_cancelled(self, is_cancelled):
+    def set_is_cancelled(self, is_cancelled: bool) -> None:
         """
         Set method for the is_cancelled
         :param is_cancelled: is_cancelled
         """
         self.__is_cancelled = is_cancelled
 
-    def get_bitpay_id_required(self):
+    def get_bitpay_id_required(self) -> bool:
         """
         Get method for the bitpay_id_required
         :return: bitpay_id_required
         """
         return self.__bitpay_id_required
 
-    def set_bitpay_id_required(self, bitpay_id_required):
+    def set_bitpay_id_required(self, bitpay_id_required: bool) -> None:
         """
         Set method for the bitpay_id_required
         :param bitpay_id_required: bitpay_id_required
         """
         self.__bitpay_id_required = bitpay_id_required
 
-    def get_rate_refresh_time(self):
-        """
-        Get method for the rate_refresh_time
-        :return: rate_refresh_time
-        """
-        return self.__rate_refresh_time
-
-    def set_rate_refresh_time(self, rate_refresh_time):
-        """
-        Set method for the rate_refresh_time
-        :param rate_refresh_time: rate_refresh_time
-        """
-        self.__rate_refresh_time = rate_refresh_time
-
-    def get_universal_codes(self):
+    def get_universal_codes(self) -> Optional[UniversalCodes]:
         """
         Get method for the universal_codes
         :return: universal_codes
         """
         return self.__universal_codes
 
-    def set_universal_codes(self, universal_codes: UniversalCodes):
+    def set_universal_codes(self, universal_codes: Optional[UniversalCodes]) -> None:
         """
         Set method for the universal_codes
         :param universal_codes: universal_codes
         """
         self.__universal_codes = universal_codes
 
-    def get_itemized_details(self):
+    def get_itemized_details(self) -> Optional[List[ItemizedDetails]]:
         """
         Get method for the itemized_details
-        :return: itemized_details
+        :return: ItemizedDetails[]
         """
-        items = []
-        for item in items:
-            if isinstance(item, ItemizedDetails):
-                items.append(item.to_json())
-            else:
-                items.append(item)
-        return items
+        return self.__itemized_details
 
-    def set_itemized_details(self, itemized_details: ItemizedDetails):
+    def set_itemized_details(self, itemized_details: List[ItemizedDetails]) -> None:
         """
         Set method for the itemized_details
         :param itemized_details: itemized_details
         """
-        items_array = []
-        for item in itemized_details:
-            if isinstance(item, ItemizedDetails):
-                items_array.append(item.to_json())
-            else:
-                items_array.append(item)
-        self.__itemized_details = items_array
+        self.__itemized_details = itemized_details
 
     # Buyer Data
 
-    def get_buyer(self):
+    def get_buyer(self) -> Optional[Buyer]:
         """
         Get method for the buyer
         :return: buyer
         """
         return self.__buyer
 
-    def set_buyer(self, buyer: Buyer):
+    def set_buyer(self, buyer: Optional[Buyer]) -> None:
         """
         Set method for the buyer
         :param buyer: buyer
         """
         self.__buyer = buyer
 
-    def to_json(self):
+    def get_buyer_sms(self) -> Optional[str]:
+        """
+        Get buyer sms
+        :return: Optional[str]
+        """
+        return self.__buyer_sms
+
+    def set_buyer_sms(self, sms: Optional[str]) -> None:
+        """
+        Set method for the buyer
+        :param sms: str
+        """
+        self.__buyer_sms = sms
+
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        supported_transaction_currencies = {}
-        for key, value in self.get_supported_transaction_currencies().to_json().items():
-            supported_transaction_currencies[key] = value.to_json()
-
-        miner_fees = {}
-        for key, value in self.get_miner_fees().to_json().items():
-            miner_fees[key] = value.to_json()
-
-        data = {
-            "currency": self.get_currency(),
-            "price": self.get_price(),
-            "token": self.get_token(),
-            "posData": self.get_pos_data(),
-            "notificationURL": self.get_notification_url(),
-            "transactionSpeed": self.get_transaction_speed(),
-            "fullNotifications": self.get_full_notifications(),
-            "notificationEmail": self.get_notification_email(),
-            "redirectURL": self.get_redirect_u_r_l(),
-            "orderId": self.get_order_id(),
-            "itemDesc": self.get_item_desc(),
-            "itemCode": self.get_item_code(),
-            "physical": self.get_physical(),
-            "paymentCurrencies": self.get_payment_currencies(),
-            "acceptanceWindow": self.get_acceptance_window(),
-            "closeURL": self.get_close_url(),
-            "buyer": self.get_buyer().to_json(),
-            "refundAddresses": self.get_refund_addresses(),
-            "id": self.get_id(),
-            "url": self.get_url(),
-            "status": self.get_status(),
-            "lowFeeDetected": self.get_low_fee_detected(),
-            "invoiceTime": self.get_invoice_time(),
-            "expirationTime": self.get_expiration_time(),
-            "transactions": self.get_transactions(),
-            "exceptionStatus": self.get_exception_status(),
-            "targetConfirmations": self.get_target_confirmations(),
-            "refundAddressRequestPending": self.get_refund_address_request_pending(),
-            "buyerProvidedEmail": self.get_buyer_provided_email(),
-            "buyerProvidedInfo": self.get_buyer_provided_info().to_json(),
-            "supportedTransactionCurrencies": supported_transaction_currencies,
-            "minerFees": miner_fees,
-            "billId": self.get_bill_id(),
-            "refundInfo": self.get_refund_info().to_json(),
-            "extendedNotifications": self.get_extended_notifications(),
-            "transactionCurrency": self.get_transaction_currency(),
-            "amountPaid": self.get_amount_paid(),
-            "exchangeRates": self.get_exchange_rates(),
-            "currentTime": self.get_current_time(),
-            "declinedAmount": self.get_declined_amount(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/models/invoice/miner_fees_item.py` & `bitpay-4.0.0/src/bitpay/models/invoice/miner_fees_item.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,85 @@
 """
 MinerFeesItem
 """
-from ...utils.key_utils import change_camel_case_to_snake_case
+from typing import Optional
+
+from bitpay.utils.key_utils import change_camel_case_to_snake_case
+from bitpay.utils.model_util import ModelUtil
 
 
 class MinerFeesItem:
     """
     The total amount of fees that the purchaser will pay to cover BitPay's
      UTXO sweep cost for an invoice. The key is the currency and the value is
       an amount in satoshis. This is referenced as "Network Cost" on an invoice,
     see this support article for more information
     """
 
     __satoshis_per_byte = None
     __total_fee = None
     __fiat_amount = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: dict) -> None:
         for key, value in kwargs.items():
             try:
+                value = ModelUtil.get_field_value(
+                    key,
+                    value,
+                    {
+                        "satoshisPerByte": "float",
+                        "totalFee": "float",
+                        "fiatAmount": "float",
+                    },
+                    {},
+                )
                 getattr(self, "set_%s" % change_camel_case_to_snake_case(key))(value)
             except AttributeError:
                 pass
 
-    def get_satoshis_per_byte(self):
+    def get_satoshis_per_byte(self) -> Optional[float]:
         """
         Get method for the satoshis_per_byte
         :return: satoshis_per_byte
         """
         return self.__satoshis_per_byte
 
-    def set_satoshis_per_byte(self, satoshis_per_byte):
+    def set_satoshis_per_byte(self, satoshis_per_byte: Optional[float]) -> None:
         """
         Set method for the satoshis_per_byte
         :param satoshis_per_byte: satoshis_per_byte
         """
         self.__satoshis_per_byte = satoshis_per_byte
 
-    def get_total_fee(self):
+    def get_total_fee(self) -> Optional[float]:
         """
         Get method for the total_fee
         :return: total_fee
         """
         return self.__total_fee
 
-    def set_total_fee(self, total_fee):
+    def set_total_fee(self, total_fee: Optional[float]) -> None:
         """
         Set method for the total_fee
         :param total_fee: total_fee
         """
         self.__total_fee = total_fee
 
-    def get_fiat_amount(self):
+    def get_fiat_amount(self) -> Optional[float]:
         """
         Get method for the fiat_amount
         :return: fiat_amount
         """
         return self.__fiat_amount
 
-    def set_fiat_amount(self, fiat_amount):
+    def set_fiat_amount(self, fiat_amount: Optional[float]) -> None:
         """
         Set method for the fiat_amount
         :param fiat_amount: fiat_amount
         """
         self.__fiat_amount = fiat_amount
 
-    def to_json(self):
+    def to_json(self) -> dict:
         """
         :return: data in json
         """
-        data = {
-            "satoshisPerByte": self.get_satoshis_per_byte(),
-            "totalFee": self.get_total_fee(),
-            "fiatAmount": self.get_fiat_amount(),
-        }
-        data = {key: value for key, value in data.items() if value}
-        return data
+        return ModelUtil.to_json(self)
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payout_query_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_query_exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     PayoutQueryException
     """
 
     __bitpay_message = "Failed to retrieve payout"
     __bitpay_code = "BITPAY-PAYOUT-GET"
     __api_code = ""
 
-    def __init__(self, message, code=123, api_code="000000"):
+    def __init__(self, message: str, code: int = 123, api_code: str = "000000"):
         """
         Construct the PayoutQueryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/rate_query_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/rate_query_exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-Rate Query Exception gets raised when request for rate retrieval gets failed .
+rate Query Exception gets raised when request for rate retrieval gets failed .
 """
 from .rates_exception import RateException
 
 
 class RateQueryException(RateException):
     """
     RateQueryException
     """
 
     __bitpay_message = "Failed to retrieve rates"
     __bitpay_code = "BITPAY-RATES-GET"
     __api_code = ""
 
-    def __init__(self, message, code=142, api_code="000000"):
+    def __init__(self, message: str, code: int = 142, api_code: str = "000000"):
         """
         Construct the RateQueryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/bill_creation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/refund_creation_exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Bill Creation Exception gets raised when request for bill creation gets failed.
+Refund Creation Exception gets raised when request for refund creation gets failed for invoice.
 """
-from .bill_exception import BillException
+from .refund_exception import RefundException
 
 
-class BillCreationException(BillException):
+class RefundCreationException(RefundException):
     """
-    BillCreationException
+    RefundCreationException
     """
 
-    __bitpay_message = "Failed to create bill"
-    __bitpay_code = "BITPAY-BILL-CREATE"
+    __bitpay_message = "Failed to create refund"
+    __bitpay_code = "BITPAY-REFUND-CREATE"
     __api_code = ""
 
-    def __init__(self, message, code=112, api_code="000000"):
+    def __init__(self, message: str, code: int = 162, api_code: str = "000000"):
         """
-        Construct the BillCreationException.
+        Construct the RefundCreationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payout_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/rates_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-Payout Exception gets raised when some unexpected error occurs while processing a request
-or trying to manage payout.
+rate Exception gets raised when some unexpected error occurs while processing a request
+or trying to manage rates.
 """
 from .bitpay_exception import BitPayException
 
 
-class PayoutException(BitPayException):
+class RateException(BitPayException):
     """
-    PayoutException
+    RateException
     """
 
-    __bitpay_message = "An unexpected error occurred while trying to manage the payout"
-    __bitpay_code = "BITPAY-PAYOUT-GENERIC"
+    __bitpay_message = "An unexpected error occurred while trying to manage the rate"
+    __bitpay_code = "BITPAY-RATES-GENERIC"
     __api_code = ""
 
-    def __init__(self, message="", code=121, api_code="000000"):
+    def __init__(self, message: str = "", code: int = 141, api_code: str = "000000"):
         """
-        Construct the PayoutException.
+        Construct the RateException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/currency_query_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/currency_query_exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     CurrencyQueryException
     """
 
     __bitpay_message = "Failed to retrieve currencies"
     __bitpay_code = "BITPAY-CURRENCY-GET"
     __api_code = ""
 
-    def __init__(self, message, code=182, api_code="000000"):
+    def __init__(self, message: str, code: int = 182, api_code: str = "000000"):
         """
         Construct the CurrencyQueryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/currency_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/currency_exception.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     __bitpay_message = (
         "An unexpected error occurred while trying to manage the currency"
     )
     __bitpay_code = "BITPAY-CURRENCY-GENERIC"
     __api_code = ""
 
-    def __init__(self, message="", code=181, api_code="000000"):
+    def __init__(self, message: str = "", code: int = 181, api_code: str = "000000"):
         """
         Construct the CurrencyException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/bill_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-Bill Exception gets raised when some unexpected error occurs while processing a request
-or trying to manage bills.
+Payout Exception gets raised when some unexpected error occurs while processing a request
+or trying to manage payout.
 """
 from .bitpay_exception import BitPayException
 
 
-class BillException(BitPayException):
+class PayoutException(BitPayException):
     """
-    BillException
+    PayoutException
     """
 
-    __bitpay_message = "An unexpected error occurred while trying to manage the bill"
-    __bitpay_code = "BITPAY-BILL-GENERIC"
+    __bitpay_message = "An unexpected error occurred while trying to manage the payout"
+    __bitpay_code = "BITPAY-PAYOUT-GENERIC"
     __api_code = ""
 
-    def __init__(self, message="", code=111, api_code="000000"):
+    def __init__(self, message: str = "", code: int = 121, api_code: str = "000000"):
         """
-        Construct the BillException.
+        Construct the PayoutException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payout_recipient_query_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_update_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-PayoutRecipientQuery Exception gets raised when request for recipient retrieval gets failed .
+PayoutRecipientUpdate Exception gets raised when it fails to update recipient
 """
-from .invoice_exception import InvoiceException
+from .payout_recipient_exception import PayoutRecipientException
 
 
-class PayoutRecipientQueryException(InvoiceException):
+class PayoutRecipientUpdateException(PayoutRecipientException):
     """
-    PayoutRecipientQueryException
+    PayoutRecipientUpdateException
     """
 
-    __bitpay_message = "Failed to retrieve payout recipient"
-    __bitpay_code = "BITPAY-PAYOUT-RECIPIENT-GET"
+    __bitpay_message = "Failed to update payout recipient"
+    __bitpay_code = "BITPAY-PAYOUT-RECIPIENT-UPDATE"
     __api_code = ""
 
-    def __init__(self, message, code=193, api_code="000000"):
+    def __init__(self, message: str, code: int = 195, api_code: str = "000000"):
         """
-        Construct the PayoutRecipientQueryException.
+        Construct the PayoutRecipientUpdateException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payoutbatch_cancellation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/invoice_cancellation_exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-PayoutBatch Cancellation exception gets raised when it fails to cancel payout batch.
+Invoice Cancellation exception gets raised when it fails to cancel invoice.
 """
-from .payout_exception import PayoutException
+from .invoice_exception import InvoiceException
 
 
-class PayoutBatchCancellationException(PayoutException):
+class InvoiceCancellationException(InvoiceException):
     """
-    PayoutBatchCancellationException
+    InvoiceCancellationException
     """
 
-    __bitpay_message = "Failed to cancel payout batch"
-    __bitpay_code = "BITPAY-PAYOUT-BATCH-CANCEL"
+    __bitpay_message = "Failed to cancel invoice object"
+    __bitpay_code = "BITPAY-INVOICE-CANCEL"
     __api_code = ""
 
-    def __init__(self, message, code=204, api_code="000000"):
+    def __init__(self, message: str, code: int = 104, api_code: str = "000000"):
         """
-        Construct the PayoutBatchCancellationException.
+        Construct the InvoiceCancellationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/refund_update_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/refund_update_exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     RefundUpdateException
     """
 
     __bitpay_message = "Failed to update refund"
     __bitpay_code = "BITPAY-REFUND-UPDATE"
     __api_code = ""
 
-    def __init__(self, message, code=164, api_code="000000"):
+    def __init__(self, message: str, code: int = 164, api_code: str = "000000"):
         """
         Construct the RefundUpdateException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/refund_query_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/refund_query_exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     RefundQueryException
     """
 
     __bitpay_message = "Failed to retrieve refund"
     __bitpay_code = "BITPAY-REFUND-GET"
     __api_code = ""
 
-    def __init__(self, message, code=163, api_code="000000"):
+    def __init__(self, message: str, code: int = 163, api_code: str = "000000"):
         """
         Construct the RefundQueryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payout_cancellation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_cancellation_exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     PayoutCancellationException
     """
 
     __bitpay_message = "Failed to cancel payout object"
     __bitpay_code = "BITPAY-PAYOUT-CANCEL"
     __api_code = ""
 
-    def __init__(self, message, code=124, api_code="000000"):
+    def __init__(self, message: str, code: int = 124, api_code: str = "000000"):
         """
         Construct the PayoutCancellationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payout_recipient_cancellation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_creation_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-PayoutRecipient Cancellation exception gets raised when it fails to cancel payout recipient.
+PayoutRecipientCreation Exception gets raised when request for recipient creation gets failed.
 """
 from .payout_recipient_exception import PayoutRecipientException
 
 
-class PayoutRecipientCancellationException(PayoutRecipientException):
+class PayoutRecipientCreationException(PayoutRecipientException):
     """
-    PayoutRecipientCancellationException
+    PayoutRecipientCreationException
     """
 
-    __bitpay_message = "Failed to cancel payout recipient"
-    __bitpay_code = "BITPAY-PAYOUT-RECIPIENT-CANCEL"
+    __bitpay_message = "Failed to create payout recipient"
+    __bitpay_code = "BITPAY-PAYOUT-RECIPIENT-SUBMIT"
     __api_code = ""
 
-    def __init__(self, message, code=194, api_code="000000"):
+    def __init__(self, message: str, code: int = 112, api_code: str = "000000"):
         """
-        Construct the PayoutRecipientCancellationException.
+        Construct the PayoutRecipientCreationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/refund_creation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/invoice_notification_exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Refund Creation Exception gets raised when request for refund creation gets failed for invoice.
+Invoice Notification Exception gets raised when webhook fails to send notification
 """
-from .refund_exception import RefundException
+from .invoice_exception import InvoiceException
 
 
-class RefundCreationException(RefundException):
+class InvoiceNotificationException(InvoiceException):
     """
-    RefundCreationException
+    InvoiceNotificationException
     """
 
-    __bitpay_message = "Failed to create refund"
-    __bitpay_code = "BITPAY-REFUND-CREATE"
+    __bitpay_message = "Failed to send invoice notification"
+    __bitpay_code = "BITPAY-INVOICE-NOTIFICATION"
     __api_code = ""
 
-    def __init__(self, message, code=162, api_code="000000"):
+    def __init__(self, message: str, code: int = 102, api_code: str = "000000"):
         """
-        Construct the RefundCreationException.
+        Construct the InvoiceNotificationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/invoice_notification_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_creation_exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Invoice Notification Exception gets raised when webhook fails to send notification
+Payout Creation Exception gets raised when request for payout creation gets failed.
 """
-from .invoice_exception import InvoiceException
+from .payout_exception import PayoutException
 
 
-class InvoiceNotificationException(InvoiceException):
+class PayoutCreationException(PayoutException):
     """
-    InvoiceNotificationException
+    PayoutCreationException
     """
 
-    __bitpay_message = "Failed to send invoice notification"
-    __bitpay_code = "BITPAY-INVOICE-NOTIFICATION"
+    __bitpay_message = "Failed to create payout"
+    __bitpay_code = "BITPAY-PAYOUT-CREATE"
     __api_code = ""
 
-    def __init__(self, message, code=102, api_code="000000"):
+    def __init__(self, message: str, code: int = 122, api_code: str = "000000"):
         """
-        Construct the InvoiceNotificationException.
+        Construct the PayoutCreationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/invoice_query_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/invoice_update_exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Invoice Query Exception gets raised when request for invoice retrieval gets failed .
+Invoice Update Exception gets raised when it fails to update invoice
 """
 from .invoice_exception import InvoiceException
 
 
-class InvoiceQueryException(InvoiceException):
+class InvoiceUpdateException(InvoiceException):
     """
-    InvoiceQueryException
+    InvoiceUpdateException
     """
 
-    __bitpay_message = "Failed to retrieve invoice"
-    __bitpay_code = "BITPAY-INVOICE-GET"
+    __bitpay_message = "Failed to update invoice"
+    __bitpay_code = "BITPAY-INVOICE-UPDATE"
     __api_code = ""
 
-    def __init__(self, message, code=103, api_code="000000"):
+    def __init__(self, message: str, code: int = 104, api_code: str = "000000"):
         """
-        Construct the InvoiceQueryException.
+        Construct the InvoiceUpdateException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/subscription_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/ledger_exception.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """
-Subscription Exception gets raised when some unexpected error occurs while processing a request
-or trying to manage subscription.
+Ledger Exception gets raised when some unexpected error occurs while processing a request
+or trying to manage ledgers.
 """
 from .bitpay_exception import BitPayException
 
 
-class SubscriptionException(BitPayException):
+class LedgerException(BitPayException):
     """
-    SubscriptionException
+    LedgerException
     """
 
-    __bitpay_message = (
-        "An unexpected error occurred while trying to manage the subscription"
-    )
-    __bitpay_code = "BITPAY-SUBSCRIPTION-GENERIC"
+    __bitpay_message = "An unexpected error occurred while trying to manage the ledger"
+    __bitpay_code = "BITPAY-LEDGER-GENERIC"
     __api_code = ""
 
-    def __init__(self, message="", code=171, api_code="000000"):
+    def __init__(self, message: str = "", code: int = 131, api_code: str = "000000"):
         """
-        Construct the SubscriptionException.
+        Construct the LedgerException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/rates_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
-Rate Exception gets raised when some unexpected error occurs while processing a request
-or trying to manage rates.
+PayoutRecipient Exception gets raised when some unexpected error occurs while processing a request
+or trying to manage recipients.
 """
 from .bitpay_exception import BitPayException
 
 
-class RateException(BitPayException):
+class PayoutRecipientException(BitPayException):
     """
-    RateException
+    PayoutRecipientException
     """
 
-    __bitpay_message = "An unexpected error occurred while trying to manage the rate"
-    __bitpay_code = "BITPAY-RATES-GENERIC"
+    __bitpay_message = (
+        "An unexpected error occurred while trying to manage the payout recipient"
+    )
+    __bitpay_code = "BITPAY-PAYOUT-RECIPIENT-GENERIC"
     __api_code = ""
 
-    def __init__(self, message="", code=141, api_code="000000"):
+    def __init__(self, message: str = "", code: int = 191, api_code: str = "000000"):
         """
-        Construct the RateException.
+        Construct the Payout Recipient Exception.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/invoice_creation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/bill_creation_exception.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Invoice Creation Exception gets raised when request for invoice creation gets failed.
+Bill Creation Exception gets raised when request for bill creation gets failed.
 """
-from .invoice_exception import InvoiceException
+from .bill_exception import BillException
 
 
-class InvoiceCreationException(InvoiceException):
+class BillCreationException(BillException):
     """
-    InvoiceCreationException
+    BillCreationException
     """
 
-    __bitpay_message = "Failed to create invoice"
-    __bitpay_code = "BITPAY-INVOICE-CREATE"
+    __bitpay_message = "Failed to create bill"
+    __bitpay_code = "BITPAY-BILL-CREATE"
     __api_code = ""
 
-    def __init__(self, message, code=102, api_code="000000"):
+    def __init__(self, message: str, code: int = 112, api_code: str = "000000"):
         """
-        Construct the InvoiceCreationException.
+        Construct the BillCreationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/settlement_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/settlement_exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     __bitpay_message = (
         "An unexpected error occurred while trying to manage the settlement"
     )
     __bitpay_code = "BITPAY-SETTLEMENTS-GENERIC"
     __api_code = ""
 
-    def __init__(self, message="", code=151, api_code="000000"):
+    def __init__(self, message: str = "", code: int = 151, api_code: str = "000000"):
         """
         Construct the SettlementException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payoutbatch_query_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_query_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-PayoutBatch Query Exception gets raised when request for payout batch retrieval gets failed .
+PayoutRecipientQuery Exception gets raised when request for recipient retrieval gets failed .
 """
-from .payout_exception import PayoutException
+from .invoice_exception import InvoiceException
 
 
-class PayoutBatchQueryException(PayoutException):
+class PayoutRecipientQueryException(InvoiceException):
     """
-    PayoutBatchQueryException
+    PayoutRecipientQueryException
     """
 
-    __bitpay_message = "Failed to retrieve payout batch"
-    __bitpay_code = "BITPAY-PAYOUT-BATCH-GET"
+    __bitpay_message = "Failed to retrieve payout recipient"
+    __bitpay_code = "BITPAY-PAYOUT-RECIPIENT-GET"
     __api_code = ""
 
-    def __init__(self, message, code=203, api_code="000000"):
+    def __init__(self, message: str, code: int = 193, api_code: str = "000000"):
         """
-        Construct the PayoutBatchQueryException.
+        Construct the PayoutRecipientQueryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/refund_cancellation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/refund_cancellation_exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     RefundCancellationException
     """
 
     __bitpay_message = "Failed to cancel refund object"
     __bitpay_code = "BITPAY-REFUND-CANCEL"
     __api_code = ""
 
-    def __init__(self, message, code=165, api_code="000000"):
+    def __init__(self, message: str, code: int = 165, api_code: str = "000000"):
         """
         Construct the RefundCancellationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/ledger_query_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/ledger_query_exception.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     LedgerQueryException
     """
 
     __bitpay_message = "Failed to retrieve ledger"
     __bitpay_code = "BITPAY-LEDGER-GET"
     __api_code = ""
 
-    def __init__(self, message, code=132, api_code="000000"):
+    def __init__(self, message: str, code: int = 132, api_code: str = "000000"):
         """
         Construct the LedgerQueryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/bill_update_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/bill_update_exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     BillUpdateException
     """
 
     __bitpay_message = "Failed to update bill"
     __bitpay_code = "BITPAY-BILL-UPDATE"
     __api_code = ""
 
-    def __init__(self, message, code=114, api_code="000000"):
+    def __init__(self, message: str, code: int = 114, api_code: str = "000000"):
         """
         Construct the BillUpdateException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/subscription_creation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/invoice_creation_exception.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Subscription Query Exception gets raised when request for subscription retrieval gets failed .
+Invoice Creation Exception gets raised when request for invoice creation gets failed.
 """
-from .subscription_exception import SubscriptionException
+from .invoice_exception import InvoiceException
 
 
-class SubscriptionCreationException(SubscriptionException):
+class InvoiceCreationException(InvoiceException):
     """
-    SubscriptionCreationException
+    InvoiceCreationException
     """
 
-    __bitpay_message = "Failed to retrieve subscriptions"
-    __bitpay_code = "BITPAY-SUBSCRIPTION-CREATE"
+    __bitpay_message = "Failed to create invoice"
+    __bitpay_code = "BITPAY-INVOICE-CREATE"
     __api_code = ""
 
-    def __init__(self, message, code=172, api_code="000000"):
+    def __init__(self, message: str, code: int = 102, api_code: str = "000000"):
         """
-        Construct the SubscriptionCreationException.
+        Construct the InvoiceCreationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/subscription_update_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/settlement_query_exception.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Subscription Update Exception gets raised when it fails to update subscription
+Settlement Query Exception gets raised when request for settlement retrieval gets failed .
 """
-from .subscription_exception import SubscriptionException
+from .settlement_exception import SettlementException
 
 
-class SubscriptionUpdateException(SubscriptionException):
+class SettlementQueryException(SettlementException):
     """
-    SubscriptionUpdateException
+    SettlementQueryException
     """
 
-    __bitpay_message = "Failed to update subscription"
-    __bitpay_code = "BITPAY-SUBSCRIPTION-UPDATE"
+    __bitpay_message = "Failed to retrieve settlements"
+    __bitpay_code = "BITPAY-SETTLEMENTS-GET"
     __api_code = ""
 
-    def __init__(self, message, code=174, api_code="000000"):
+    def __init__(self, message: str, code: int = 152, api_code: str = "000000"):
         """
-        Construct the SubscriptionUpdateException.
+        Construct the SettlementQueryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/ledger_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/refund_exception.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-Ledger Exception gets raised when some unexpected error occurs while processing a request
-or trying to manage ledgers.
+Refund Exception gets raised when some unexpected error occurs while processing a request
+or trying to manage refund.
 """
 from .bitpay_exception import BitPayException
 
 
-class LedgerException(BitPayException):
+class RefundException(BitPayException):
     """
-    LedgerException
+    RefundException
     """
 
-    __bitpay_message = "An unexpected error occurred while trying to manage the ledger"
-    __bitpay_code = "BITPAY-LEDGER-GENERIC"
+    __bitpay_message = "An unexpected error occurred while trying to manage the refund"
+    __bitpay_code = "BITPAY-REFUND-GENERIC"
     __api_code = ""
 
-    def __init__(self, message="", code=131, api_code="000000"):
+    def __init__(self, message: str = "", code: int = 161, api_code: str = "000000"):
         """
-        Construct the LedgerException.
+        Construct the RefundException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payoutbatch_creation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_notification_exception.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Payout Creation Exception gets raised when request for payout batch creation gets failed.
+Payout Notification Exception gets raised when webhook fails to send notification
 """
 from .payout_exception import PayoutException
 
 
-class PayoutBatchCreationException(PayoutException):
+class PayoutNotificationException(PayoutException):
     """
-    PayoutBatchCreationException
+    PayoutNotificationException
     """
 
-    __bitpay_message = "Failed to create payout batch"
-    __bitpay_code = "BITPAY-PAYOUT-BATCH-CREATE"
+    __bitpay_message = "Failed to send payout notification"
+    __bitpay_code = "BITPAY-PAYOUT-NOTIFICATION"
     __api_code = ""
 
-    def __init__(self, message, code=202, api_code="000000"):
+    def __init__(self, message: str, code: int = 126, api_code: str = "000000"):
         """
-        Construct the PayoutBatchCreationException.
+        Construct the PayoutNotificationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payout_recipient_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_cancellation_exception.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
-PayoutRecipient Exception gets raised when some unexpected error occurs while processing a request
-or trying to manage recipients.
+PayoutRecipient Cancellation exception gets raised when it fails to cancel payout recipient.
 """
-from .bitpay_exception import BitPayException
+from .payout_recipient_exception import PayoutRecipientException
 
 
-class PayoutRecipientException(BitPayException):
+class PayoutRecipientCancellationException(PayoutRecipientException):
     """
-    PayoutRecipientException
+    PayoutRecipientCancellationException
     """
 
-    __bitpay_message = (
-        "An unexpected error occurred while trying to manage the payout recipient"
-    )
-    __bitpay_code = "BITPAY-PAYOUT-RECIPIENT-GENERIC"
+    __bitpay_message = "Failed to cancel payout recipient"
+    __bitpay_code = "BITPAY-PAYOUT-RECIPIENT-CANCEL"
     __api_code = ""
 
-    def __init__(self, message="", code=191, api_code="000000"):
+    def __init__(self, message: str, code: int = 194, api_code: str = "000000"):
         """
-        Construct the Payout Recipient Exception.
+        Construct the PayoutRecipientCancellationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/settlement_query_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/refund_notification_exception.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Settlement Query Exception gets raised when request for settlement retrieval gets failed .
+Refund Notification Exception gets raised when webhook fails to send notification
 """
-from .settlement_exception import SettlementException
+from .refund_exception import RefundException
 
 
-class SettlementQueryException(SettlementException):
+class RefundNotificationException(RefundException):
     """
-    SettlementQueryException
+    RefundNotificationException
     """
 
-    __bitpay_message = "Failed to retrieve settlements"
-    __bitpay_code = "BITPAY-SETTLEMENTS-GET"
+    __bitpay_message = "Failed to send refund notification"
+    __bitpay_code = "BITPAY-REFUND-NOTIFICATION"
     __api_code = ""
 
-    def __init__(self, message, code=152, api_code="000000"):
+    def __init__(self, message: str, code: int = 166, api_code: str = "000000"):
         """
-        Construct the SettlementQueryException.
+        Construct the RefundNotificationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payoutbatch_notification_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/invoice_payment_exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-PayoutBatch Notification Exception gets raised when webhook fails to send notification
+Invoice Payment exception gets raised when it fails to pay invoice.
 """
-from .payout_exception import PayoutException
+from .invoice_exception import InvoiceException
 
 
-class PayoutBatchNotificationException(PayoutException):
+class InvoicePaymentException(InvoiceException):
     """
-    PayoutBatchNotificationException
+    InvoicePaymentException
     """
 
-    __bitpay_message = "Failed to send payout batch notification"
-    __bitpay_code = "BITPAY-PAYOUT-BATCH-NOTIFICATION"
+    __bitpay_message = "Failed to pay invoice"
+    __bitpay_code = "BITPAY-INVOICE-PAY-UPDATE"
     __api_code = ""
 
-    def __init__(self, message, code=206, api_code="000000"):
+    def __init__(self, message: str, code: int = 107, api_code: str = "000000"):
         """
-        Construct the PayoutBatchNotificationException.
+        Construct the InvoicePaymentException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payout_creation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/payout_recipient_notification_exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Payout Creation Exception gets raised when request for payout creation gets failed.
+PayoutRecipientNotification Exception gets raised when webhook fails to send notification
 """
-from .payout_exception import PayoutException
+from .payout_recipient_exception import PayoutRecipientException
 
 
-class PayoutCreationException(PayoutException):
+class PayoutRecipientNotificationException(PayoutRecipientException):
     """
-    PayoutCreationException
+    PayoutRecipientNotificationException
     """
 
-    __bitpay_message = "Failed to create payout"
-    __bitpay_code = "BITPAY-PAYOUT-CREATE"
+    __bitpay_message = "Failed to send payout recipient notification"
+    __bitpay_code = "BITPAY-PAYOUT-RECIPIENT-NOTIFICATION"
     __api_code = ""
 
-    def __init__(self, message, code=122, api_code="000000"):
+    def __init__(self, message: str, code: int = 196, api_code: str = "000000"):
         """
-        Construct the PayoutCreationException.
+        Construct the PayoutRecipientNotificationException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payout_notification_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/wallet_query_exception.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Payout Notification Exception gets raised when webhook fails to send notification
+Wallet Query Exception gets raised when a user fails to retrieve wallets
 """
-from .payout_exception import PayoutException
+from .wallet_exception import WalletException
 
 
-class PayoutNotificationException(PayoutException):
+class WalletQueryException(WalletException):
     """
-    PayoutNotificationException
+    WalletQueryException
     """
 
-    __bitpay_message = "Failed to send payout notification"
-    __bitpay_code = "BITPAY-PAYOUT-NOTIFICATION"
+    __bitpay_message = "Failed to retrieve supported wallets"
+    __bitpay_code = "BITPAY-WALLET-GET"
     __api_code = ""
 
-    def __init__(self, message, code=126, api_code="000000"):
+    def __init__(self, message: str, code: int = 183, api_code: str = "000000"):
         """
-        Construct the PayoutNotificationException.
+        Construct the WalletQueryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/bill_delivery_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/bill_delivery_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     BillDeliveryException
     """
 
     __bitpay_message = "Failed to deliver bill"
     __bitpay_code = "BITPAY-BILL-DELIVERY"
     __api_code = ""
 
-    def __init__(self, message, code=115, api_code="000000"):
+    def __init__(self, message: str, code: int = 115, api_code: str = "000000"):
         """
         Construct the BillDeliveryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/refund_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/bill_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-Refund Exception gets raised when some unexpected error occurs while processing a request
-or trying to manage refund.
+Bill Exception gets raised when some unexpected error occurs while processing a request
+or trying to manage bills.
 """
 from .bitpay_exception import BitPayException
 
 
-class RefundException(BitPayException):
+class BillException(BitPayException):
     """
-    RefundException
+    BillException
     """
 
-    __bitpay_message = "An unexpected error occurred while trying to manage the refund"
-    __bitpay_code = "BITPAY-REFUND-GENERIC"
+    __bitpay_message = "An unexpected error occurred while trying to manage the bill"
+    __bitpay_code = "BITPAY-BILL-GENERIC"
     __api_code = ""
 
-    def __init__(self, message="", code=161, api_code="000000"):
+    def __init__(self, message: str = "", code: int = 111, api_code: str = "000000"):
         """
-        Construct the RefundException.
+        Construct the BillException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payoutbatch_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/bill_query_exception.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
-PayoutBatch Exception gets raised when some unexpected error occurs while processing a request
-or trying to manage payout batch.
+Bill Query Exception gets raised when request for bill retrieval gets failed .
 """
-from .bitpay_exception import BitPayException
+from .bill_exception import BillException
 
 
-class PayoutBatchException(BitPayException):
+class BillQueryException(BillException):
     """
-    PayoutBatchException
+    BillQueryException
     """
 
-    __bitpay_message = (
-        "An unexpected error occurred while trying to manage the payout batch"
-    )
-    __bitpay_code = "BITPAY-PAYOUT-BATCH-GENERIC"
+    __bitpay_message = "Failed to retrieve bill"
+    __bitpay_code = "BITPAY-BILL-GET"
     __api_code = ""
 
-    def __init__(self, message="", code=201, api_code="000000"):
+    def __init__(self, message: str, code: int = 113, api_code: str = "000000"):
         """
-        Construct the PayoutBatchException.
+        Construct the BillQueryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/invoice_cancellation_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/invoice_query_exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-Invoice Cancellation exception gets raised when it fails to cancel invoice.
+Invoice Query Exception gets raised when request for invoice retrieval gets failed .
 """
 from .invoice_exception import InvoiceException
 
 
-class InvoiceCancellationException(InvoiceException):
+class InvoiceQueryException(InvoiceException):
     """
-    InvoiceCancellationException
+    InvoiceQueryException
     """
 
-    __bitpay_message = "Failed to cancel invoice object"
-    __bitpay_code = "BITPAY-INVOICE-CANCEL"
+    __bitpay_message = "Failed to retrieve invoice"
+    __bitpay_code = "BITPAY-INVOICE-GET"
     __api_code = ""
 
-    def __init__(self, message, code=104, api_code="000000"):
+    def __init__(self, message: str, code: int = 103, api_code: str = "000000"):
         """
-        Construct the InvoiceCancellationException.
+        Construct the InvoiceQueryException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/bitpay_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/bitpay_exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     BitPayException
     """
 
     __bitpay_message = "Unexpected Bitpay exception."
     __bitpay_code = "BITPAY-GENERIC"
     __api_code = ""
 
-    def __init__(self, message, code=100, api_code="000000"):
+    def __init__(self, message: str, code: int = 100, api_code: str = "000000"):
         """
         Construct the BillUpdateException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
         super().__init__(message, code)
 
-    def get_api_code(self):
+    def get_api_code(self) -> str:
         """
         :return: Error code provided by the BitPay REST API
         """
         return self.__api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/bill_query_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/invoice_exception.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
-Bill Query Exception gets raised when request for bill retrieval gets failed .
+Invoice Exception gets raised when some unexpected error occurs while processing a request
+or trying to manage invoice.
 """
-from .bill_exception import BillException
+from .bitpay_exception import BitPayException
 
 
-class BillQueryException(BillException):
+class InvoiceException(BitPayException):
     """
-    BillQueryException
+    InvoiceException
     """
 
-    __bitpay_message = "Failed to retrieve bill"
-    __bitpay_code = "BITPAY-BILL-GET"
+    __bitpay_message = "An unexpected error occurred while trying to manage the invoice"
+    __bitpay_code = "BITPAY-INVOICE-GENERIC"
     __api_code = ""
 
-    def __init__(self, message, code=113, api_code="000000"):
+    def __init__(self, message: str = "", code: int = 100, api_code: str = "000000"):
         """
-        Construct the BillQueryException.
+        Construct the InvoiceException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/exceptions/payout_recipient_update_exception.py` & `bitpay-4.0.0/src/bitpay/exceptions/wallet_exception.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
-PayoutRecipientUpdate Exception gets raised when it fails to update recipient
+Wallet Exception gets raised when some unexpected error occurs while processing a request
+or trying to manage wallet.
 """
-from .payout_recipient_exception import PayoutRecipientException
+from .bitpay_exception import BitPayException
 
 
-class PayoutRecipientUpdateException(PayoutRecipientException):
+class WalletException(BitPayException):
     """
-    PayoutRecipientUpdateException
+    WalletException
     """
 
-    __bitpay_message = "Failed to update payout recipient"
-    __bitpay_code = "BITPAY-PAYOUT-RECIPIENT-UPDATE"
+    __bitpay_message = "An unexpected error occurred while trying to manage the wallet"
+    __bitpay_code = "BITPAY-WALLET-GENERIC"
     __api_code = ""
 
-    def __init__(self, message, code=195, api_code="000000"):
+    def __init__(self, message: str = "", code: int = 181, api_code: str = "000000"):
         """
-        Construct the PayoutRecipientUpdateException.
+        Construct the WalletException.
 
         :param message: The Exception message to throw.
         :param code: [optional] The Exception code to throw.
         :param api_code: [optional] The API Exception code to throw.
         """
         message = self.__bitpay_code + ": " + self.__bitpay_message + ":" + message
         self.__api_code = api_code
```

### Comparing `bitpay-3.4.2203/src/bitpay/bitpay_setup.py` & `bitpay-4.0.0/src/bitpay/bitpay_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,78 @@
 import os
 import json
+from typing import Optional
+
 import requests
 
-from bitpay.utils.key_utils import *
-from bitpay.exceptions.bitpay_exception import BitPayException
+from utils.key_utils import *
+from exceptions.bitpay_exception import BitPayException
 
 # Will be set to Test otherwise
 private_key_name = "private_key.pem"  # Add here the name for your Private key
-private_key_path = os.path.join(os.path.abspath(os.curdir), private_key_name)
+private_key_path: Optional[str] = os.path.join(
+    os.path.abspath(os.curdir), private_key_name
+)
 plain_private_key = None
 proxy = None
 api_url = None
 environment = None
 merchant_token = None
 payout_token = None
 
 
-def select_env():
+def select_env() -> None:
     global environment
     try:
         print("Select target environment: ")
         target_environment = input("Press T for testing or P for production: \n")
 
         if target_environment.lower() == "t":
             environment = "Test"
         elif target_environment.lower() == "p":
             environment = "Prod"
         else:
             select_env()
 
-        set_environment(environment)
+        set_environment(environment)  # type: ignore
         select_create_key()
     except BitPayException as exe:
         print(exe)
 
 
-def set_environment(env):
+def set_environment(env: str) -> None:
     global api_url
     if env == "Test":
         api_url = "https://test.bitpay.com"
     else:
         api_url = "https://bitpay.com"
 
 
-def select_create_key():
+def select_create_key() -> None:
     try:
         input_value = input(
             "Press enter to generate a brand new key or enter your private key location:"
         )
         if input_value == "":
             create_new_key()
         else:
             load_key()
     except BitPayException as exe:
         print(exe)
 
 
-def create_new_key():
+def create_new_key() -> None:
     try:
-        private_key = generate_pem()
+        private_key = generate_pem()  # type: ignore
         store_key(private_key)
     except BitPayException as exe:
         print(exe)
 
 
-def store_key(private_key):
+def store_key(private_key: str) -> None:
     global plain_private_key, private_key_path
     try:
         print("Select the way you want to store your private key:")
         input_value = input(
             "Press F for storing in a pem file or T for plain text in your config file: "
         )
 
@@ -85,33 +89,33 @@
             select_tokens(private_key)
         else:
             store_key(private_key)
     except BitPayException as exe:
         print(exe)
 
 
-def select_tokens(private_key):
+def select_tokens(private_key: str) -> None:
     try:
         print("Select the tokens that you would like to request:")
         input_value = input("Press M for merchant, P for payout, or B for both: \n")
         if input_value.lower() in ["m", "p", "b"]:
             print("Requesting Tokens... \n")
             request_tokens(input_value.lower(), private_key)
         else:
             select_tokens(private_key)
     except BitPayException as exe:
         print(exe)
 
 
-def request_tokens(token_type, private_key):
+def request_tokens(token_type: str, private_key: str) -> None:
     global merchant_token
     global payout_token
 
     try:
-        sin = get_sin_from_pem(private_key)
+        sin = get_sin_from_pem(private_key)  # type: ignore
         url = "%s/tokens" % api_url
         headers = {"content-type": "application/json", "X-accept-version": "2.0.0"}
 
         if token_type in ["m", "b"]:
             print("Requesting Merchant token... \n")
             facade = "merchant"
             payload = {"id": sin, "facade": facade}
@@ -144,15 +148,15 @@
                 )
 
         update_config_file()
     except BitPayException as exe:
         print(exe)
 
 
-def update_config_file():
+def update_config_file() -> None:
     try:
         config = {
             "BitPayConfiguration": {
                 "Environment": environment,
                 "EnvConfig": {
                     environment: {
                         "PrivateKeyPath": private_key_path,
@@ -183,14 +187,14 @@
             "\r\nOnce you have this Pairing Code/s approved you can move the generated files to a secure location "
             "and start using the Client.\r\n"
         )
     except BitPayException as exe:
         print(exe)
 
 
-def load_key():
+def load_key() -> None:
     # TODO: Need to implement this function
     pass
 
 
 if __name__ == "__main__":
     select_env()
```

### Comparing `bitpay-3.4.2203/src/bitpay.egg-info/PKG-INFO` & `bitpay-4.0.0/src/bitpay.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: bitpay
-Version: 3.4.2203
+Version: 4.0.0
 Summary: Accept bitcoin with BitPay
 Home-page: https://github.com/bitpay/python-bitpay-client
+Download-URL: https://github.com/bitpay/python-bitpay-client/tarball/v3.4.2203
 Author: Antonio Buedo
 Author-email: sales-engineering@bitpay.com
-License: UNKNOWN
-Download-URL: https://github.com/bitpay/python-bitpay-client/tarball/v3.4.2203
-Description:         Python Library for integrating with BitPay
-                
-                This library is a simple way to integrate your application with
-                BitPay for taking Bitcoin payments. It exposes three basic 
-                functions, authenticating with BitPay, creating invoices, 
-                and retrieving invoices. It is not meant as a replacement for 
-                the entire BitPay API. However, the key_utils module contains
-                all of the tools you need to use the BitPay API for other
-                purposes.
-                
-                This version requires only Python 3.8.
-                
 Keywords: bitcoin,payments,crypto,cash,ethereum,online payments
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Office/Business :: Financial
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+        Python Library for integrating with BitPay
+        
+        This library is a simple way to integrate your application with
+        BitPay for taking Bitcoin payments. It exposes three basic 
+        functions, authenticating with BitPay, creating invoices, 
+        and retrieving invoices. It is not meant as a replacement for 
+        the entire BitPay API. However, the key_utils module contains
+        all of the tools you need to use the BitPay API for other
+        purposes.
+        
+        This version requires Python 3.8 or higher.
+
```

### Comparing `bitpay-3.4.2203/src/bitpay.egg-info/SOURCES.txt` & `bitpay-4.0.0/src/bitpay.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,33 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 src/bitpay/__init__.py
 src/bitpay/bitpay_setup.py
 src/bitpay/client.py
 src/bitpay/config.py
-src/bitpay/env.py
-src/bitpay/tokens.py
+src/bitpay/environment.py
 src/bitpay.egg-info/PKG-INFO
 src/bitpay.egg-info/SOURCES.txt
 src/bitpay.egg-info/dependency_links.txt
 src/bitpay.egg-info/requires.txt
 src/bitpay.egg-info/top_level.txt
+src/bitpay/clients/__init__.py
+src/bitpay/clients/bill_client.py
+src/bitpay/clients/bitpay_client.py
+src/bitpay/clients/currency_client.py
+src/bitpay/clients/invoice_client.py
+src/bitpay/clients/ledger_client.py
+src/bitpay/clients/payout_client.py
+src/bitpay/clients/payout_recipient_client.py
+src/bitpay/clients/rate_client.py
+src/bitpay/clients/refund_client.py
+src/bitpay/clients/settlement_client.py
+src/bitpay/clients/wallet_client.py
 src/bitpay/exceptions/__init__.py
 src/bitpay/exceptions/bill_creation_exception.py
 src/bitpay/exceptions/bill_delivery_exception.py
 src/bitpay/exceptions/bill_exception.py
 src/bitpay/exceptions/bill_query_exception.py
 src/bitpay/exceptions/bill_update_exception.py
 src/bitpay/exceptions/bitpay_exception.py
@@ -37,91 +49,75 @@
 src/bitpay/exceptions/payout_query_exception.py
 src/bitpay/exceptions/payout_recipient_cancellation_exception.py
 src/bitpay/exceptions/payout_recipient_creation_exception.py
 src/bitpay/exceptions/payout_recipient_exception.py
 src/bitpay/exceptions/payout_recipient_notification_exception.py
 src/bitpay/exceptions/payout_recipient_query_exception.py
 src/bitpay/exceptions/payout_recipient_update_exception.py
-src/bitpay/exceptions/payoutbatch_cancellation_exception.py
-src/bitpay/exceptions/payoutbatch_creation_exception.py
-src/bitpay/exceptions/payoutbatch_exception.py
-src/bitpay/exceptions/payoutbatch_notification_exception.py
-src/bitpay/exceptions/payoutbatch_query_exception.py
 src/bitpay/exceptions/rate_query_exception.py
 src/bitpay/exceptions/rates_exception.py
 src/bitpay/exceptions/refund_cancellation_exception.py
 src/bitpay/exceptions/refund_creation_exception.py
 src/bitpay/exceptions/refund_exception.py
 src/bitpay/exceptions/refund_notification_exception.py
 src/bitpay/exceptions/refund_query_exception.py
 src/bitpay/exceptions/refund_update_exception.py
 src/bitpay/exceptions/settlement_exception.py
 src/bitpay/exceptions/settlement_query_exception.py
-src/bitpay/exceptions/subscription_creation_exception.py
-src/bitpay/exceptions/subscription_exception.py
-src/bitpay/exceptions/subscription_query_exception.py
-src/bitpay/exceptions/subscription_update_exception.py
 src/bitpay/exceptions/wallet_exception.py
 src/bitpay/exceptions/wallet_query_exception.py
 src/bitpay/models/__init__.py
 src/bitpay/models/currency.py
 src/bitpay/models/facade.py
-src/bitpay/models/Rate/__init__.py
-src/bitpay/models/Rate/rate.py
-src/bitpay/models/Rate/rates.py
 src/bitpay/models/bill/__init__.py
 src/bitpay/models/bill/bill.py
 src/bitpay/models/bill/bill_status.py
 src/bitpay/models/bill/item.py
 src/bitpay/models/invoice/__init__.py
 src/bitpay/models/invoice/buyer.py
 src/bitpay/models/invoice/buyer_provided_info.py
 src/bitpay/models/invoice/invoice.py
+src/bitpay/models/invoice/invoice_event_token.py
 src/bitpay/models/invoice/invoice_status.py
 src/bitpay/models/invoice/itemized_details.py
 src/bitpay/models/invoice/miner_fees.py
 src/bitpay/models/invoice/miner_fees_item.py
 src/bitpay/models/invoice/refund.py
 src/bitpay/models/invoice/refund_info.py
-src/bitpay/models/invoice/refund_params.py
 src/bitpay/models/invoice/refund_status.py
 src/bitpay/models/invoice/shopper.py
 src/bitpay/models/invoice/supported_transaction_currencies.py
 src/bitpay/models/invoice/supported_transaction_currency.py
+src/bitpay/models/invoice/transaction.py
 src/bitpay/models/invoice/universal_codes.py
 src/bitpay/models/ledger/__init__.py
 src/bitpay/models/ledger/buyer.py
 src/bitpay/models/ledger/ledger.py
 src/bitpay/models/ledger/ledger_entry.py
 src/bitpay/models/payout/__init__.py
 src/bitpay/models/payout/payout.py
-src/bitpay/models/payout/payout_batch.py
-src/bitpay/models/payout/payout_instruction.py
-src/bitpay/models/payout/payout_instruction_btc_summary.py
-src/bitpay/models/payout/payout_instruction_transaction.py
-src/bitpay/models/payout/payout_received_info.py
-src/bitpay/models/payout/payout_received_info_address.py
+src/bitpay/models/payout/payout_group.py
+src/bitpay/models/payout/payout_group_failed.py
 src/bitpay/models/payout/payout_recipient.py
 src/bitpay/models/payout/payout_recipients.py
 src/bitpay/models/payout/payout_status.py
 src/bitpay/models/payout/payout_transaction.py
-src/bitpay/models/payout/recipient_reference_method.py
 src/bitpay/models/payout/recipient_status.py
+src/bitpay/models/rate/__init__.py
+src/bitpay/models/rate/rate.py
+src/bitpay/models/rate/rates.py
 src/bitpay/models/settlement/__init__.py
 src/bitpay/models/settlement/invoice_data.py
 src/bitpay/models/settlement/payout_info.py
 src/bitpay/models/settlement/refund_info.py
 src/bitpay/models/settlement/settlement.py
 src/bitpay/models/settlement/settlement_ledger_entry.py
 src/bitpay/models/settlement/with_holdings.py
-src/bitpay/models/subscription/__init__.py
-src/bitpay/models/subscription/bill_data.py
-src/bitpay/models/subscription/item.py
-src/bitpay/models/subscription/subscription.py
-src/bitpay/models/subscription/subscription_status.py
 src/bitpay/models/wallet/__init__.py
 src/bitpay/models/wallet/currencies.py
 src/bitpay/models/wallet/currency_qr.py
 src/bitpay/models/wallet/wallet.py
 src/bitpay/utils/__init__.py
+src/bitpay/utils/guid_generator.py
 src/bitpay/utils/key_utils.py
-src/bitpay/utils/rest_cli.py
+src/bitpay/utils/model_util.py
+src/bitpay/utils/token_container.py
```

