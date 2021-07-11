# SlowMotion
SlowMotion Fortnite Exploit

if (settings::slowmo) {
							if (LocalPawn && PlayerController)
							{
								if (SDK::Utilities::SpoofCall(SteamHelper::GetAsyncKeyState, VK_SHIFT))
								{
									*reinterpret_cast<float*>(reinterpret_cast<PBYTE>(LocalPawn) + Offsets::CustomTimeDialation) = 0.3;
								}
								else
								{
									*reinterpret_cast<float*>(reinterpret_cast<PBYTE>(LocalPawn) + Offsets::CustomTimeDialation) = 1;
								}
							}
}
