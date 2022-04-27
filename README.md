
This table based of information from:
* https://infocenter.nordicsemi.com/index.jsp?topic=%2Fcom.nordic.infocenter.s132.api.v2.0.0%2Fgroup___b_l_e___h_c_i___s_t_a_t_u_s___c_o_d_e_s.html
* http://allmydroids.blogspot.com/2015/06/android-ble-error-status-codes-explained.html

(New) - is mark for last interpretation of this status code

Status|	Status Hex	|Description|	Explanation
---|-------|-----------------------------------------------------|---------
0	|0x00	|BLE_HCI_STATUS_CODE_SUCCESS	                     |Everything ok!:)
1	|0x01	|BLE_HCI_STATUS_CODE_UNKNOWN_BTLE_COMMAND	         |              
1	|0x01	|CONNECTION_PRIORITY_HIGH               	         |(New)Connection parameter update - Request a high priority, low latency connection. An application should only request high priority connection parameters to transfer large amounts of data over LE quickly. Once the transfer is complete, the application should request BluetoothGatt#CONNECTION_PRIORITY_BALANCED connection parameters to reduce energy use.                            
2	|0x02	|BLE_HCI_STATUS_CODE_UNKNOWN_CONNECTION_IDENTIFIER	 |              
2	|0x02	|CONNECTION_PRIORITY_LOW_POWER                   	 |(New)Connection parameter update - Request low power, reduced data rate connection parameters.       
3	|0x03	|GATT_WRITE_NOT_PERMITTED                        	 |GATT write operation is not permitted              
5	|0x05	|BLE_HCI_AUTHENTICATION_FAILURE	                     |Insufficient authentication for a given operation            
6	|0x06	|BLE_HCI_STATUS_CODE_PIN_OR_KEY_MISSING	             |        
6	|0x06	|GATT_REQUEST_NOT_SUPPORTED         	             |The given request is not supported             
7	|0x07	|BLE_HCI_MEMORY_CAPACITY_EXCEEDED	                 |        
7	|0x07	|GATT_INVALID_OFFSET            	                 |A read or write operation was requested with an invalid offset           
8	|0x08	|BLE_HCI_CONNECTION_TIMEOUT                          |Could not establish a connection in specified period. Maybe device is currently connected to something else?
8	|0x08	|GATT_INSUFFICIENT_AUTHORIZATION                     |Insufficient authorization for a given operation
12	|0x0C	|BLE_HCI_STATUS_CODE_COMMAND_DISALLOWED	             |
13	|0xD	|GATT_INVALID_ATTRIBUTE_LENGTH       	             |A write operation exceeds the maximum length of the attribute
15	|0xF	|GATT_INSUFFICIENT_ENCRYPTION       	             |Insufficient encryption for a given operation 
18	|0x12	|BLE_HCI_STATUS_CODE_INVALID_BTLE_COMMAND_PARAMETERS |
19	|0x13	|BLE_HCI_REMOTE_USER_TERMINATED_CONNECTION           |Remote device has forced a disconnect.
20	|0x14	|BLE_HCI_REMOTE_DEV_TERMINATION_DUE_TO_LOW_RESOURCES |                                                           
21	|0x15	|BLE_HCI_REMOTE_DEV_TERMINATION_DUE_TO_POWER_OFF	 |                                                       
22	|0x16	|BLE_HCI_LOCAL_HOST_TERMINATED_CONNECTION	         |                                               
26	|0x1A	|BLE_HCI_UNSUPPORTED_REMOTE_FEATURE	                 |                                       
30	|0x1E	|BLE_HCI_STATUS_CODE_INVALID_LMP_PARAMETERS	         |                                               
31	|0x1F	|BLE_HCI_STATUS_CODE_UNSPECIFIED_ERROR	             |                                           
34	|0x22	|BLE_HCI_STATUS_CODE_LMP_RESPONSE_TIMEOUT	         |                                               
36	|0x24	|BLE_HCI_STATUS_CODE_LMP_PDU_NOT_ALLOWED	         |                                               
40	|0x28	|BLE_HCI_INSTANT_PASSED	                             |                           
41	|0x29	|BLE_HCI_PAIRING_WITH_UNIT_KEY_UNSUPPORTED	         |                                               
42	|0x2A	|BLE_HCI_DIFFERENT_TRANSACTION_COLLISION	         |                                               
58	|0x3A	|BLE_HCI_CONTROLLER_BUSY	                         |                               
59	|0x3B	|BLE_HCI_CONN_INTERVAL_UNACCEPTABLE	                 |                                       
60	|0x3C	|BLE_HCI_DIRECTED_ADVERTISER_TIMEOUT	             |                                           
61	|0x3D	|BLE_HCI_CONN_TERMINATED_DUE_TO_MIC_FAILURE	         |                                               
62	|0x3E	|BLE_HCI_CONN_FAILED_TO_BE_ESTABLISHED	             |                                           
128	|0x80	|GATT_NO_RESSOURCES	                                 |                       
129	|0x81	|GATT_INTERNAL_ERROR	                             |                           
130	|0x82	|GATT_WRONG_STATE	                                 |                       
131	|0x83	|GATT_DB_FULL	                                     |                   
132	|0x84	|GATT_BUSY	                                         |               
133	|0x85	|GATT_ERROR	                                         |Can be anything, from device not in Range to a random error.
135	|0x87	|GATT_ILLEGAL_PARAMETER	                             |
137	|0x89	|GATT_AUTH_FAIL                                      |A GATT operation failed, errors other than the above
143	|0x8f	|GATT_CONNECTION_CONGESTED                           |A remote device connection is congested.
257 |0x101  |GATT_FAILURE                                        |