# UnrealSyntax


# How to get DeltaTime 
// Returns the frame delta time in seconds adjusted by e.g. time dilation
* GetWorld()->GetDeltaSeconds();

# Draw Debug (Sphere in this case*)
// Draws a sphere in the world (World, Location, Radius, Segments, Color, {}, LifeTime, {}, Thickness)
* DrawDebugSphere(GetWorld(), GetActorLocation(), 25.f, 12, FColor::Red, false, 0.1f, 0, 2.f);


# Print Function - Displays on the screen ("Print" in BP)
//A simple print  ({}, LifeTime, Color, Message)
* GEngine->AddOnScreenDebugMessage(-1, 2.0f, FColor::Blue, TEXT("Hello World!");

# UE_LOG - Displays in the "Output Log"
// Prints "Hello World" as an Warning
* UE_LOG(LogTemp, Warning, TEXT("Hello World!"));
---
// Prints "1+1=2" as an Error
* int MyInt = 2;
* UE_LOG(LogTemp, Error, TEXT("1+1=%i"), MyInt)


# Get Viewport size (ex. 1920x1080)
* FVector2D ViewportSize;
* GEngine->GameViewport->GetViewportSize(ViewportSize); // Returns an FVector2D
