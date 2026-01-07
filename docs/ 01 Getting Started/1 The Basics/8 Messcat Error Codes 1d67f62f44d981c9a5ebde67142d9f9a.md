# Messcat Error Codes

Article Description: A consolidated list of all the error codes in Messcat
Last Updated: December 3, 2024

This is a consolidated list of all the error codes in Messcat. Please search for your error to understand what might be causing it

| Error Code | Description | HTTP Status Code |
| --- | --- | --- |
| noTierChangeNonAuto | Cannot change tier of an account that is not auto charged | 400 |
| accountApprovalReq | Account must be approved before updating business info | 400 |
| leaveBeforeDeleteGroup | You must leave the group before deleting it | 400 |
| phoneNumReq | Phone number required | 400 |
| openAccountReq | Require at least one open account to check if user exists | 400 |
| nothingToUpdate | Nothing to update | 400 |
| invalidName | Given value is not a valid name | 400 |
| cannotForwardMsgs | Cannot forward "note" or "pending" or "errored" messages | 400 |
| cannotForwardAction | Cannot forward action messages | 400 |
| cannotUpdateOtherMsg | Cannot update a message that is not from you | 400 |
| noUpdateNonPending | Cannot update a message that is not pending or errored out | 400 |
| canOnlyEditNotes | Can only edit notes | 400 |
| onlyMarkNotesResolved | Can only mark notes as resolved | 400 |
| noTsChangeWithStatus | Cannot change timestamp with current status of message | 400 |
| statusReqAllQuery | Need to supply a status with "all" query | 400 |
| cannotForceReloadMsgs | Cannot force reload all messages | 400 |
| noMsgReloadingSupport | This account does not support reloading messages from the platform | 400 |
| noFetchMsgAllAccChat | Cannot fetch messages for all accounts and a specific chat | 400 |
| templateReqNewConv | A template is required to start a new conversation | 400 |
| badTextTryAgain | Bad text, try again! | 400 |
| noButtonsWithPoll | Cannot send buttons with url or phone number as poll | 400 |
| nothingToDelete | Nothing to delete | 400 |
| missingProduct | No products to forward sync | 400 |
| invalidAccType | Account type does not support template submission | 400 |
| invalidAccountType | Invalid account type | 400 |
| notRegAlibaba | Account is not registered as an alibaba-cams-v2 account | 400 |
| accountActivated | Account must be activated | 400 |
| invalidAttachmentUrl | Invalid attachment url | 400 |
| invalidAttachment | Invalid attachment URL provided | 400 |
| incorrectMimeType | Attachments must have the correct mimetype. Received an unexpected mimetype. | 400 |
| missingLocation | Missing location property of the location attachment | 400 |
| shortPhoneNum | Phone number must be at least 5 digits | 400 |
| attachmentsNotSupported | Attachments not supported | 400 |
| buttonsNotSupported | Buttons not supported | 400 |
| productsNotSupported | Products not supported | 400 |
| messageMustHaveText | Message must have text | 400 |
| noSimultaneousBtnAttach | Cannot send message with buttons and attachment at the same time | 400 |
| urlPhoneBtnsNotSupported | Sending URL & phone number buttons directly is not supported | 400 |
| pollsNotSupported | Polls not supported on WABA | 400 |
| notSupportedOnWABA | Products not supported on WABA | 400 |
| emptyPhoneNumber | Empty phone number provided | 400 |
| failedGetCodeScanQR | Failed to get code from WhatsApp. Please try scanning the QR code | 400 |
| invalidChatId | Invalid chat ID | 400 |
| contactsBaseUrlsOnly | Contacts only support base64 encoded URLs | 400 |
| expectedJsonCursor | Expected stringified JSON cursor | 400 |
| invalidJsonCursor | Invalid JSON cursor | 400 |
| noTeamCreatorChange | Cannot alter the team creator! | 400 |
| noDeleteOwnUser | Cannot delete your own user! | 400 |
| noAlterOwnUser | Cannot alter your own user! | 400 |
| unsupportedLoginMethod | Login method not supported | 400 |
| invalidOtherParameter | Invalid other parameter | 400 |
| phoneNumReqForOtp | Phone number required for OTP | 400 |
| teamIdIsReq | teamId is required | 400 |
| noStoresInBoutir | No Stores In Boutir Account | 400 |
| noPhoneNumFound | No Phone Number Found | 400 |
| missingEmailLogin | Email address missing from Google login | 400 |
| invalidRequest | Invalid request | 400 |
| templateNotFound | No template found for given templateID | 400 |
| noBotsForBotId | No bots for given botId | 400 |
| noActionsForBotid | No actions for given botId | 400 |
| noTextOrTitleBotID | No message text or title for given botId | 400 |
| templateIdIsReqToLink | Template ID is required to link | 400 |
| startingActionReq | Bot needs to have a starting action before it can be submitted for review | 400 |
| msgReqInStartingAction | Starting action must contain a message | 400 |
| missingStartingAction | Bot has no starting action! | 400 |
| invalidCursor | Invalid cursor | 400 |
| unknownActionid | Unknown starting actionID | 400 |
| webhookMethodReq | Webhook trigger method expected | 400 |
| delayLoopInActions | Found delay loop in those actions | 400 |
| unsupportedTargetType | Specified target type not supported | 400 |
| undefinedPropertyPath | Result of PropertyPath is undefined | 400 |
| InvalidPropertyPathId | Result of PropertyPath is not a single ID or list of ids | 400 |
| BtnActionNotFound | The button action could not be found | 400 |
| campaignInProgressStop | Campaign already in progress, "stop" the campaign first | 400 |
| noRecipientsLeft | No recipients left to broadcast | 400 |
| noRecipientsForCampaign | No recipients present for the given campaign | 400 |
| stringifiedJsonReq | Expected stringified JSON cursor | 400 |
| missingTrigger | There is no trigger associated | 400 |
| qRCodeUrlIsReq | QR code url is required | 400 |
| missingAuthInPayment | Payment system has no auth | 400 |
| UnsupportedServiceProducts | Specified service integration does not support products | 400 |
| nameConditionInvalid | Cannot condition on specified name | 400 |
| emptyNameCondition | Condition with specified name has no values | 400 |
| invalidValueTypeError | Invalid value type provided. | 400 |
| InvalidNameConditionValues | Condition with specified name cannot have given values | 400 |
| unknownConditions | Unknown conditions specified | 400 |
| paymentIntegrationNotFound | Payment integration with specified paymentIntegrationId does not exist | 400 |
| invalidStartTimeFormat | Malformed startTime! must be in 24h format | 400 |
| invalidEndTimeFormat | Malformed endTime! must be in 24h format | 400 |
| malformedEndtimeMissing | Malformed endTime! missing | 400 |
| missingKeywords | Missing keywords | 400 |
| missingUser | Could not find user | 400 |
| unavailablePaymentId | No payment ID available | 400 |
| noAutoChargeApi | This account is not an auto-charged API product, it cannot be removed | 400 |
| NonScalableApi | Account not part of scalable API plan | 400 |
| duplicateTierMembership | Account already belongs to "${tier}", nothing to do | 400 |
| invalidSubsId | Invalid subscription id | 400 |
| wrongCategoryUpdate | Cannot update to a product in a different category | 400 |
| nonSubUpdateOnly | Purchase is not a subscription. Can only update subscriptions | 400 |
| noPartnerAdminTeam | No partner admin set for this team | 400 |
| noCreditToAvail | No credit to avail | 400 |
| noExtraDaysAllowed | Cannot add extra days to one-time product | 400 |
| invalidPurchaseDetail | Malformed purchaseDetail! | 400 |
| invalidTeam | Malformed team! | 400 |
| invalidTeamMember | Malformed teamMember! | 400 |
| attachmentNotEncrypted | Attachment is not encrypted | 400 |
| unauthorisedForWebhook | Unauthorised for webhook | 401 |
| invalidExpiredRefresh | Invalid or expired refresh token | 401 |
| invalidPhoneNumPwd | Invalid phone number/password combination | 401 |
| unknownOtp | Unknown OTP | 401 |
| tokenNotFound | Token not found | 401 |
| oTPNotFound | OTP not found | 401 |
| invalidPhoneOrOtp | Invalid phone or otp | 401 |
| invalidIntegrationCode | Invalid integration code | 401 |
| invalidWebhookSecret | Invalid webhook secret | 401 |
| invalidIntegrationId | Invalid integration ID | 401 |
| invalidOrderId | Invalid order id | 401 |
| noToken | No token | 401 |
| quotaExhausted | Accounts Quota Exhausted | 403 |
| notAuthorizedToUpdate | You need the TEAMMEMBERS_UPDATE scope to access this data | 403 |
| messageQuotaExhausted | Message Quota Exhausted | 403 |
| cannotSendBroadcast | Cannot send to broadcast lists | 403 |
| noScopePermission | You do not have permission to grant these scopes! | 403 |
| captchaCheckFailed | Captcha check failed | 403 |
| userNotFoundInTeam | Cannot find your user in the team | 403 |
| noScopeUpdateAccess | You do not have enough access to update these scopes on this team member | 403 |
| extraIDsToUpdate | Received extra member IDs to update | 403 |
| scopesNotPresent | Scopes not present | 403 |
| maxMembersReached | This team already has the maximum number of members! | 403 |
| insufficientScope | You do not have access to this | 403 |
| userNotInPartnership | This user is not part of your partnership | 403 |
| noChangeNonPartner | Cannot change for this user as it is not a partnership account | 403 |
| noChangeForUser | Cannot change for this user | 403 |
| cannotUpdateFields | Cannot update these fields | 403 |
| noAccessReqScopes | You do not have access to certain scopes you requested | 403 |
| insufficientScopes | You do not have the required scopes to perform this action | 403 |
| insufficientAccess | Insufficient Access | 403 |
| maxPurchasesReached | Max purchases reached | 403 |
| forbidden | Forbidden | 403 |
| OwnReferralNotAllowed | Cannot use your own referral code | 403 |
| noAccountsFound | No accounts found | 404 |
| couldNotFindAnAccount | Could not find an account | 404 |
| missingAccountInTeam | Could not find given account in your team | 404 |
| missingProductID | Product with given id not found in your team | 404 |
| missingEntity | Could not find the specified entity. | 404 |
| chatNotFound | Original chat not found | 404 |
| originalMsgNotFound | Original message not found | 404 |
| expectedOriginalData | Expected message to have original data | 404 |
| failedFindIdInChat | Failed to find id in chat given chatId | 404 |
| adminNotFound | Your partner admin team was not found | 404 |
| invalidTeamOrNoAccess | Either the team specified is invalid, or you do not have access | 404 |
| contactNotFound | Contact not found | 404 |
| teamNotFound | Team not found | 404 |
| notFound | Not Found | 404 |
| missingAccountId | Could not find specified accountId in your team | 404 |
| campaignNotFound | Campaign not found | 404 |
| missingDataPoint | Could not find data point | 404 |
| missingSecretId | Could not find tracking by specified secretId | 404 |
| missingPaymentSystem | Payment system not found | 404 |
| UnsupportedWebhookPayment | Payment system cannot handle webhook | 404 |
| missingTrackingId | Could not find tracking with specified trackingId | 404 |
| missingMetadataTeamId | Could not find metadata with specified teamId | 404 |
| noQrFound | No QrCode returned | 404 |
| noSuchChatbotId | No such chatbot id | 404 |
| chatbotNotFound | Chatbot not found | 404 |
| missingChatbothName | Chatbot does not exist with name | 404 |
| missingChatbotId | Could not find chatbot id | 404 |
| invalidCoupanCode | Specified coupon code is invalid | 404 |
| productCodeNotFound | Product code not found | 404 |
| messageNotFound | Message with specified not found | 404 |
| attachmentNotFound | Attachment not found | 404 |
| 2closeBeforeDelete | Account must be closed before deleting | 409 |
| cannotConnectInThisState | Cannot connect in given state | 409 |
| cannotSetReadEquals | Cannot set read equals to given value when chat is same | 409 |
| cannotSetActionEquals | Cannot set action equals to given value when chat is same | 409 |
| accountAlreadyOpen | Account already open | 409 |
| duplicateOpenRequest | Duplicate open request for the specified account. | 409 |
| userAlreadyInTeam | User is already a member of this team! | 409 |
| noPassChangeForSso | Cannot change password for Google/Facebook/Boutir login | 409 |
| userAlreadyRegistered | This user is already registered! Please login, if you have forgotten your password, press "forgot password" | 409 |
| flowNameAlreadyExists | A flow with the same name already exists | 409 |
| sameNameFolderExists | A folder with the same name already exists | 409 |
| DuplicateIDError | Specified ID has already been taken | 409 |
| tiktokCookiesReq | Cannot open account without TikTok cookies | 418 |
| cannotFetchMsgs | Cannot fetch messages in direction other than "before" | 418 |
| noContactInfoFound | Cannot fetch contact info for phone number | 418 |
| notSupported | Not supported | 418 |
| mismatchAccWrkrType | The specified account is not running on the specified worker | 424 |
| accountNotOpenMsg | Account not open, cannot send message | 428 |
| openAccountReqForDetail | Account needs to be open to fetch order details | 428 |
| accountNotOpen | Account must be open to sync products | 428 |
| accountNotRunning | Account not running | 428 |
| accountNotActivated | Account not activated | 428 |
| noConnectionInstance | No connection instance | 428 |
| lastMsgTooLongAgo | Last msg too long ago | 428 |
| notOpenConnection | Connection not open yet | 428 |
| noMoreOTPsTryLater | Cannot send more OTPs. Please try again in some time | 429 |
| notImplemented | Not implemented | 500 |
| noTeammatesFound | No teammates found | 500 |
| accountReqRoundRobin | Account must be provided for round-robin assign type | 500 |
| noTeammatesForAssign | No teammates found for smart assign contact | 500 |
| noWorkerAvailable | No worker available. Contact Support. | 500 |
| senderUserIdNotSet | Sender user ID not set | 500 |
| messageIdNotSet | Message ID not set | 500 |
| entityMutationFailed | Failed to run single mutation on current entity | 500 |
| noTeamMembers | The specified team has no team members. | 500 |
| missingMethod | The requested method is not implemented. | 500 |
| templateCreateNoId | Template create did not return ID | 500 |
| couldNotGetWaba | Could not get waba | 500 |
| phoneNumNotFound | Could not find phone number | 500 |
| invalidModification | Invalid modification | 500 |
| reqFieldsForSearch | Contact name, platform names and phone number are required to set search | 500 |
| writeCollectionError | Error writing to given collection | 500 |
| sendgridApiKeyNotSet | SENDGRID_API_KEY not set specified partner | 500 |
| cannotRegisterGroup | Cannot register a group | 500 |
| allWebPushFailed | All Web push failed | 500 |
| gptIssueTryAgain | Oops seems GPT ran into problems, please try again | 500 |
| contactFilterConflict | Cannot use both contactFilters and addTags/removeTags | 500 |
| recvNonJsonPayload | Recv non JSON payload | 500 |
| filterConflictExcludedTags | Cannot use both contactFilters and recipientTags/excludedRecipientTags | 500 |
| FailedToGetPayexToken | Error getting Payex access token | 500 |
| paymentCreationFailed | Error creating payment intent | 500 |
| transactionDetailsError | Error getting transaction details | 500 |
| invalidAuthType | Invalid auth type | 500 |
| InvalidWebhook | Invalid webhook. No metadata or txn_id or payment_intent | 500 |
| requestInProgress | Async requests in progress, please wait for them to finish before starting a new one | 500 |
| invalidDay | Invalid Day | 500 |
| trialNotAvailable | Free trial not available! | 500 |
| subItemNotFoundInvoice | Could not find the subscription item in the invoice | 500 |
| teamHasNoCreator | Team has no creator | 500 |
| emptyQuotaNoOwner | Event message-quota-empty without ownerId | 500 |
| tokenServiceNotFound | Service refreshToken/serviceTeamId does not exist! | 500 |